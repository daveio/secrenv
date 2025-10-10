# frozen_string_literal: true

require "bundler/gem_tasks"
require "standard/rake"

require "rb_sys/extensiontask"

task build: :compile

GEMSPEC = Gem::Specification.load("secrenv.gemspec")

RbSys::ExtensionTask.new("secrenv", GEMSPEC) do |ext|
  ext.lib_dir = "lib/secrenv"
end

task default: %i[compile standard]

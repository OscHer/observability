# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  # Seahaven será el bastión desde el que lanzaremos los playbooks
  config.vm.define "seahaven" do |seahaven|
    seahaven.vm.box = "debian/bullseye64"
    seahaven.vm.hostname = "seahaven"
  end

  # Truman: nodo observado (sutil, verdad?)
  config.vm.define "truman" do |truman|
    truman.vm.box = "generic/rhel8"
    truman.vm.hostname = "truman"
  end

  # Christof: colector de información
  config.vm.define "christof" do |christof|
    christof.vm.box = "generic/rhel8"
    christof.vm.hostname = "christof"
  end
end

# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  # Seahaven será el bastión desde el que lanzaremos los playbooks
  config.vm.define "seahaven" do |seahaven|
    seahaven.vm.box = "debian/bullseye64"
  end

  # Truman: nodo observado (sutil, verdad?)
  config.vm.define "truman" do |truman|
    truman.vm.box = "generic/rhel8"
  end

  # Christof: colector de información
  config.vm.define "christof" do |cristof|
    cristof.vm.box = "generic/rhel8"
  end
end

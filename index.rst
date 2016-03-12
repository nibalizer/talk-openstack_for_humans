
.. Secure Peer Networking with TINC slides file, created by
   hieroglyph-quickstart on Sun Nov 15 21:40:13 2015.


====================
OpenStack For Humans
====================

.. figure:: _static/cascadia_logo.png
   :align: left
   :width: 400px

Spencer Krum, IBM

March 12, 2016

@nibalizer

.. note::

   * Who am I
   * What do I work on
   * github
   * This talk is my version of an introduction to openstack
   * demystify
   * objective truths
   * no vendor pitch
   * i want you to know the words when openstack is being discussed
   * I'll also show you how to use it


Portland
========

.. figure:: _static/mt_hood.jpg
   :align: center




.. slide:: 
   :level: 2

   .. figure:: _static/openstack-cloud-software-vertical-large.png
      :align: center

Agenda
======

* Introduction
* OpenStack Word Definitions
* OpenStack UX
* Examples


Who Am I?
=========


.. note::
    * Sysop
    * PSU
    * Work at IBM
    * I build the infrastructure that tests openstack, jenkins, code hosting
    * Access to a good half dozen clouds
    * boot nodes all the time
    * Working at IBM to deploy a cloud



What is OpenStack
=================

.. rst-class:: build

* Python Daemons
* Infrastructure as a Service
* Open Source


.. note::
    * Python daemon that takes in rest api and then causes other things to happen
    * Some kind of a programmable thing that does stuff that datacenter techs used to do
    * Tickets!
    * Ticket to get a vm
    * Rest API to get a vm
    * Apache 2


What OpenStack is Not
=====================

.. rst-class:: build

* Hypervisor
* Amazon


.. note::
    * Xen, Kvm, Virtualbox, Vmware these are hypervisors
    * Amazon web services, its not that and its not compatible


The Four Opens
==============

* Open Source
* Open Design
* Open Development
* Open Community


.. note::
    * Not Open Core, Apache2
    * Design is open and open to contributors
    * The development is done in the open with open tooling
    * The discussion and voting and technical direction is all transparent
    * There is a CoC



History
=======

* Started 2010
* Collaboration between Rackspace and NASA
* Releases every 6 months
* Mitaka is comming out RSN

.. note::
    * I started working on it in 2014


Fast Facts
==========

* ~600 git repos
* ~7k emails / 6 mo
* 20k commits / 6 mo
* 100k reviews / 6 mo

.. note::
    * openstack development is freaking huge


Basic Things you can ask an OpenStack to do
===========================================

* Make a vm
* Destroy a vm
* Set a dns record
* Store a file
* Create a 2T disk and attach it to a vm
* Create a mysql database


Less Basic things you can ask an OpenStack to do
================================================

* Snapshot a vm
* Upload an image to boot new vms from
* Create an L2 network segment that several vms are all tapped into


Primary Services
================

* Nova
* Neutron
* Glance
* Cinder
* Keystone
* Swift
* Trove
* Designate

.. note::
    * These are the things that we really need to be up
    * Our CI system is home grown and awesome


Iaas UX
=======

.. rst-class:: build

* Invisible/No Interaction
* Web UI
* Command line utility
* Deployment Tool
* Library

.. note::
    * OpenStack has a UX Team
    * What is cloud ux





References
==========

* All infra repos: http://git.openstack.org/cgit/openstack-infra/
* Main Control repo: http://git.openstack.org/cgit/openstack-infra/system-config
* ansible-puppet role: http://git.openstack.org/cgit/openstack-infra/system-config
* Apply test: http://git.openstack.org/cgit/openstack-infra/system-config/tree/tools/apply-test.sh
* OpenStack CI http://docs.openstack.org/infra/openstackci/
* Diskimage-Builder http://docs.openstack.org/developer/diskimage-builder/

References (cont)
=================

* ELK Upgrade Playbook: https://review.openstack.org/#/c/238185/
* Ansible puppetdb glue: http://git.openstack.org/cgit/openstack-infra/ansible-puppet/tree/library/puppet_post_puppetdb
* Json puppet report processor: http://git.openstack.org/cgit/openstack-infra/system-config/tree/modules/openstack_project/lib/puppet/reports/puppetdb_file.rb

References: shas
================

* Drive puppet from ssh: edaa31ebbda09fb03baf1d18b64f5fa996188745
* Move from ssh to ansible: 034f37c32aed27d8000e1dc3a8a3d36022bcd12a
* Public hiera: 1624692402d2148ab7d6dd9e5642fb0b34ec7209



Thank You + Questions
=====================

.. figure:: _static/spencer_face.jpg
   :align: left

Spencer Krum

IBM

@nibalizer

nibz@spencerkrum.com

https://git.openstack.org/cgit/openstack-infra/publications



.. slide:: Show Bullets Incrementally
   :level: 2

   .. rst-class:: build

   - Adding the ``build`` class to a container
   - To incrementally show its contents
   - Remember that *Sphinx* maps the basic ``class`` directive to
     ``rst-class``

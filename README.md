# orchestrator

## Description

The Orchestrator is part of the SODALITE Runtime Layer. It is in charge of the deployment and reconfiguration of SODALITE applications. It takes an IaC blueprint (i.e., a TOSCA+Ansible playbooks file) and performs the deployment of the applications on heterogeneous infrastructures.

The most important features of the Orchestrator are:

* Deployments on HPC and cloud
* Support of TOSCA declarative workflows
* Support of TOSCA CSAR blueprints
* ...

![Architecture](documentation/orchestrator.png)

The orchestrator building block is composed of the orchestrator itself and drivers to connect to the different targets. Currently, the orchestrator supports the deployment of applications on Openstack and we have certain support for HPC through Torque.

This repository contains two sub-repositories:
- xOpera as the orchestrator
- ALDE as the HPC driver. ALDE is a fork from the [TANGO](http://tango-project.eu/) project. It provides a uniform REST API to manage HPC workload managers and applications deployed on them (currently, Slurm). In SODALITE, ALDE is being extended to support Torque.

## Software requirements

* python3 and virtual environments

## Installation

Both projects contains detailed installation instructions. In general, you need to:

1. Create the virtual environment:

        $ python3 -m venv <env-dir>
        $ source <env-dir>/bin/activate

2. Install the pip packages

        $ cd <project-dir>
        $ pip install

3. Run!

## Usage

Check individual repositories on usage guides. 


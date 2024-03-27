# Introduction

## About Equinix Labs

Equinix Labs offers workshops, proof of concepts, and tools for exploring and bootstrapping Equinix digital infrastructure including Fabric, Metal, and Network Edge.

## About the workshop

Welcome to the workshop on provisioning Equinix infrastructure using Pulumi. Throughout this workshop, we will explore the capabilities of Pulumi, leveraging its versatility through multi-language and multi-cloud support. Our demonstration will focus on utilizing a Pulumi template written in Python to establish a private connection from a new Equinix Fabric Cloud Router to Google Cloud Platform (GCP). We will utilize the Pulumi providers for Equinix and GCP.

It's important to note that currently, there's a limitation with the GCP provider, as it does not include the option to update pre-created BGP configuration, necessitating a manual step to add the BGP peer ASN. Nevertheless, this functionality is achievable using the GCP API and its Python SDK. Therefore, in this example, we will explore extending the functionality of Pulumi providers with programming logic, achieving end-to-end automation.

The goals of this workshop are:
  
* How to use Pulumi and Equinix together
* Defining and deploying Equinix resources using popular programming languages
* Establishing a private interconnection to a Cloud Service Provider
* How to extend the functionality of Pulumi providers

## Workshop agenda

This workshop is split into four parts:

| Part | Title | Duration |
| - | - | - |
| 1 | Setup | 15 minutes |
| 2 | Provisioning | 15 minutes |
| 3 | Application | 10 minutes |
| 4 | Conclusion | 5 minutes |


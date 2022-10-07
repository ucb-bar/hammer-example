# Hammer Example

This repo contains a minimal example of a RTL -> GDS flow using Hammer, either of the OpenROAD or Cadence toolchains, and the ASAP7 or Skywater 130 PDKs.

## Setup

### Environment

This repo has environment (commercial CAD tool paths and license servers) configs for Berkeley EECS compute nodes (BWRC, Millennium, and instructional machines) in `env`.
Add a file for your environment if you are using commercial tools in `env`.

### PDKs

#### ASAP7

If you're using a Berkeley EECS compute node, find the ASAP7 install configs in `pdks/asap7-{a,bwrc,inst]}.yml`.

If you're using another environment:

1. Clone the [asap7 repo](https://github.com/The-OpenROAD-Project/asap7)
2. Create an ASAP7 install config modeled after the configs in `pdks/asap7{a,bwrc,inst}.yml`

### CAD Tools

### Designs

## Running Hammer

```shell
hammer-vlsi -e env/a-env.yml -p pdks/asap7-a.yml -p test.yml
```

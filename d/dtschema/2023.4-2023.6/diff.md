# Comparing `tmp/dtschema-2023.4.tar.gz` & `tmp/dtschema-2023.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtschema-2023.4.tar", last modified: Tue Apr 11 22:26:58 2023, max compression
+gzip compressed data, was "dtschema-2023.6.tar", last modified: Mon Jun 26 23:23:10 2023, max compression
```

## Comparing `dtschema-2023.4.tar` & `dtschema-2023.6.tar`

### file list

```diff
@@ -1,142 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.529180 dtschema-2023.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.485180 dtschema-2023.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.497180 dtschema-2023.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-11 22:26:40.000000 dtschema-2023.4/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-11 22:26:40.000000 dtschema-2023.4/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-11 22:26:40.000000 dtschema-2023.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-11 22:26:40.000000 dtschema-2023.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-04-11 22:26:58.529180 dtschema-2023.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-04-11 22:26:40.000000 dtschema-2023.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.497180 dtschema-2023.4/dtschema/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14921 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/dtb.py
--rw-r--r--   0 runner    (1001) docker     (123)    43162 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.505180 dtschema-2023.4/dtschema/meta-schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/base.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/boolean.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/cell.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/clocks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/core.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/dma.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/gpios.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/hwlock.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/iio.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/interrupts.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/iommu.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/items.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/keywords.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/mailbox.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/nodes.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/nvmem.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/phy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/power-domain.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/pwm.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/reset.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/string-array.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/meta-schemas/vendor-props.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.513180 dtschema-2023.4/dtschema/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/aliases.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/bootph.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.513180 dtschema-2023.4/dtschema/schemas/bus/
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/bus/qemu,platform.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/cache-controller.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/cache.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9188 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/chosen.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.513180 dtschema-2023.4/dtschema/schemas/clock/
--rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/clock/clock.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/cpu.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/cpus.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.513180 dtschema-2023.4/dtschema/schemas/dma/
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/dma/dma.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/dt-core.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.513180 dtschema-2023.4/dtschema/schemas/gpio/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/gpio/gpio-consumer.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/gpio/gpio-hog.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/gpio/gpio.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/graph.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.513180 dtschema-2023.4/dtschema/schemas/hwlock/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/hwlock/hwlock-consumer.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.513180 dtschema-2023.4/dtschema/schemas/i2c/
--rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/i2c/i2c-controller.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.513180 dtschema-2023.4/dtschema/schemas/iio/
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/iio/iio-consumer.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/iio/iio.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/interconnects.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/interrupt-controller.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/interrupts.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.517180 dtschema-2023.4/dtschema/schemas/iommu/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/iommu/iommu.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.517180 dtschema-2023.4/dtschema/schemas/isa/
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/isa/isa-bridge.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/isa/isa-bus.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.517180 dtschema-2023.4/dtschema/schemas/mbox/
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/mbox/mbox-consumer.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/memory.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/msi-consumer.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.517180 dtschema-2023.4/dtschema/schemas/opp/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/opp/opp.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.517180 dtschema-2023.4/dtschema/schemas/options/
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/options/u-boot.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/options.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.517180 dtschema-2023.4/dtschema/schemas/pci/
--rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/pci/pci-bus.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/pci/pci-iommu.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.517180 dtschema-2023.4/dtschema/schemas/phy/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/phy/phy-consumer.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/phy/phy-provider.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.517180 dtschema-2023.4/dtschema/schemas/pinctrl/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/pinctrl/pinctrl-consumer.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.517180 dtschema-2023.4/dtschema/schemas/power-domain/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/power-domain/power-domain-consumer.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/property-units.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.521180 dtschema-2023.4/dtschema/schemas/pwm/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/pwm/pwm-consumer.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/reg.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.521180 dtschema-2023.4/dtschema/schemas/reset/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/reset/reset.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/root-node.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/serial.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/simple-bus.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-04-11 22:26:40.000000 dtschema-2023.4/dtschema/schemas/types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 22:26:58.000000 dtschema-2023.4/dtschema/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.497180 dtschema-2023.4/dtschema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-04-11 22:26:58.000000 dtschema-2023.4/dtschema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-04-11 22:26:58.000000 dtschema-2023.4/dtschema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 22:26:58.000000 dtschema-2023.4/dtschema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-11 22:26:58.000000 dtschema-2023.4/dtschema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 22:26:58.000000 dtschema-2023.4/dtschema.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-04-11 22:26:40.000000 dtschema-2023.4/example-schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 22:26:58.529180 dtschema-2023.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1638 2023-04-11 22:26:40.000000 dtschema-2023.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.525180 dtschema-2023.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-11 22:26:40.000000 dtschema-2023.4/test/bootphases.dts
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-11 22:26:40.000000 dtschema-2023.4/test/child-node-fail.dts
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-11 22:26:40.000000 dtschema-2023.4/test/child-node.dts
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-11 22:26:40.000000 dtschema-2023.4/test/conditionals-allof-fail.dts
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-11 22:26:40.000000 dtschema-2023.4/test/conditionals-allof-pass.dts
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-11 22:26:40.000000 dtschema-2023.4/test/conditionals-single-fail.dts
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-11 22:26:40.000000 dtschema-2023.4/test/conditionals-single-pass.dts
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-04-11 22:26:40.000000 dtschema-2023.4/test/device-fail.dts
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-11 22:26:40.000000 dtschema-2023.4/test/device.dts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.525180 dtschema-2023.4/test/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-11 22:26:40.000000 dtschema-2023.4/test/schemas/bad-example.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-11 22:26:40.000000 dtschema-2023.4/test/schemas/child-node-example.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-11 22:26:40.000000 dtschema-2023.4/test/schemas/conditionals-allof-example.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-11 22:26:40.000000 dtschema-2023.4/test/schemas/conditionals-single-example.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-04-11 22:26:40.000000 dtschema-2023.4/test/schemas/good-example.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-11 22:26:40.000000 dtschema-2023.4/test/simple-bus-fail.dts
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-11 22:26:40.000000 dtschema-2023.4/test/simple-bus-pass.dts
--rwxr-xr-x   0 runner    (1001) docker     (123)     6384 2023-04-11 22:26:40.000000 dtschema-2023.4/test/test-dt-validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 22:26:58.529180 dtschema-2023.4/tools/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1347 2023-04-11 22:26:40.000000 dtschema-2023.4/tools/dt-check-compatible
--rwxr-xr-x   0 runner    (1001) docker     (123)     2128 2023-04-11 22:26:40.000000 dtschema-2023.4/tools/dt-doc-validate
--rwxr-xr-x   0 runner    (1001) docker     (123)     2628 2023-04-11 22:26:40.000000 dtschema-2023.4/tools/dt-extract-example
--rwxr-xr-x   0 runner    (1001) docker     (123)     1908 2023-04-11 22:26:40.000000 dtschema-2023.4/tools/dt-extract-props
--rwxr-xr-x   0 runner    (1001) docker     (123)     1519 2023-04-11 22:26:40.000000 dtschema-2023.4/tools/dt-mk-schema
--rwxr-xr-x   0 runner    (1001) docker     (123)     6206 2023-04-11 22:26:40.000000 dtschema-2023.4/tools/dt-prop-populate
--rwxr-xr-x   0 runner    (1001) docker     (123)     6934 2023-04-11 22:26:40.000000 dtschema-2023.4/tools/dt-validate
--rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-04-11 22:26:40.000000 dtschema-2023.4/tools/dtb2py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1225 2023-04-11 22:26:40.000000 dtschema-2023.4/tools/extract-compatibles
--rwxr-xr-x   0 runner    (1001) docker     (123)     2135 2023-04-11 22:26:40.000000 dtschema-2023.4/tools/yaml-format
--rwxr-xr-x   0 runner    (1001) docker     (123)      766 2023-04-11 22:26:40.000000 dtschema-2023.4/tools/yaml2json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:23:10.406568 dtschema-2023.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:23:10.378568 dtschema-2023.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:23:10.382568 dtschema-2023.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-26 23:22:57.000000 dtschema-2023.6/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-26 23:22:57.000000 dtschema-2023.6/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-26 23:22:57.000000 dtschema-2023.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-26 23:22:57.000000 dtschema-2023.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-06-26 23:23:10.406568 dtschema-2023.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-26 23:22:57.000000 dtschema-2023.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:23:10.386568 dtschema-2023.6/dtschema/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15065 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/dtb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16102 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/fixups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:23:10.390568 dtschema-2023.6/dtschema/meta-schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/meta-schemas/base.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/meta-schemas/boolean.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/meta-schemas/cell.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/meta-schemas/clocks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/meta-schemas/core.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/meta-schemas/dma.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/meta-schemas/gpios.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/meta-schemas/hwlock.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/meta-schemas/iio.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/meta-schemas/interrupts.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/meta-schemas/iommu.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/meta-schemas/items.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/meta-schemas/keywords.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/meta-schemas/mailbox.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/meta-schemas/nodes.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/meta-schemas/nvmem.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/meta-schemas/phy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/meta-schemas/power-domain.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/meta-schemas/pwm.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/meta-schemas/reset.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/meta-schemas/string-array.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/meta-schemas/vendor-props.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:23:10.394568 dtschema-2023.6/dtschema/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/aliases.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/bootph.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:23:10.394568 dtschema-2023.6/dtschema/schemas/bus/
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/bus/qemu,platform.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/cache-controller.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/cache.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9188 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/chosen.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:23:10.394568 dtschema-2023.6/dtschema/schemas/clock/
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/clock/clock.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/cpu.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/cpus.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:23:10.394568 dtschema-2023.6/dtschema/schemas/dma/
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/dma/dma.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/dt-core.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:23:10.394568 dtschema-2023.6/dtschema/schemas/gpio/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/gpio/gpio-consumer.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/gpio/gpio-hog.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/gpio/gpio.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/graph.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:23:10.394568 dtschema-2023.6/dtschema/schemas/hwlock/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/hwlock/hwlock-consumer.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:23:10.394568 dtschema-2023.6/dtschema/schemas/i2c/
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/i2c/i2c-controller.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:23:10.398568 dtschema-2023.6/dtschema/schemas/iio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/iio/iio-consumer.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/iio/iio.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/interconnects.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/interrupt-controller.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/interrupts.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:23:10.398568 dtschema-2023.6/dtschema/schemas/iommu/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/iommu/iommu.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:23:10.398568 dtschema-2023.6/dtschema/schemas/isa/
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/isa/isa-bridge.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/isa/isa-bus.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:23:10.398568 dtschema-2023.6/dtschema/schemas/mbox/
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/mbox/mbox-consumer.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/memory.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/msi-consumer.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:23:10.398568 dtschema-2023.6/dtschema/schemas/opp/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/opp/opp.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:23:10.398568 dtschema-2023.6/dtschema/schemas/options/
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/options/u-boot.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/options.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:23:10.398568 dtschema-2023.6/dtschema/schemas/pci/
+-rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/pci/pci-bus.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/pci/pci-iommu.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:23:10.398568 dtschema-2023.6/dtschema/schemas/phy/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/phy/phy-consumer.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/phy/phy-provider.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:23:10.398568 dtschema-2023.6/dtschema/schemas/pinctrl/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/pinctrl/pinctrl-consumer.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:23:10.398568 dtschema-2023.6/dtschema/schemas/power-domain/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/power-domain/power-domain-consumer.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/property-units.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:23:10.398568 dtschema-2023.6/dtschema/schemas/pwm/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/pwm/pwm-consumer.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/reg.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:23:10.398568 dtschema-2023.6/dtschema/schemas/reset/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/reset/reset.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/root-node.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/serial.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/simple-bus.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/schemas/types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    15951 2023-06-26 23:22:57.000000 dtschema-2023.6/dtschema/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 23:23:10.000000 dtschema-2023.6/dtschema/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:23:10.386568 dtschema-2023.6/dtschema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-06-26 23:23:10.000000 dtschema-2023.6/dtschema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-06-26 23:23:10.000000 dtschema-2023.6/dtschema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 23:23:10.000000 dtschema-2023.6/dtschema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-26 23:23:10.000000 dtschema-2023.6/dtschema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 23:23:10.000000 dtschema-2023.6/dtschema.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-06-26 23:22:57.000000 dtschema-2023.6/example-schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 23:23:10.406568 dtschema-2023.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1638 2023-06-26 23:22:57.000000 dtschema-2023.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:23:10.402568 dtschema-2023.6/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-26 23:22:57.000000 dtschema-2023.6/test/bootphases.dts
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-26 23:22:57.000000 dtschema-2023.6/test/child-node-fail.dts
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-26 23:22:57.000000 dtschema-2023.6/test/child-node.dts
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-26 23:22:57.000000 dtschema-2023.6/test/conditionals-allof-fail.dts
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-26 23:22:57.000000 dtschema-2023.6/test/conditionals-allof-pass.dts
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-26 23:22:57.000000 dtschema-2023.6/test/conditionals-single-fail.dts
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-26 23:22:57.000000 dtschema-2023.6/test/conditionals-single-pass.dts
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-06-26 23:22:57.000000 dtschema-2023.6/test/device-fail.dts
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-26 23:22:57.000000 dtschema-2023.6/test/device.dts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:23:10.402568 dtschema-2023.6/test/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-26 23:22:57.000000 dtschema-2023.6/test/schemas/bad-example.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-26 23:22:57.000000 dtschema-2023.6/test/schemas/child-node-example.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-26 23:22:57.000000 dtschema-2023.6/test/schemas/conditionals-allof-example.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-26 23:22:57.000000 dtschema-2023.6/test/schemas/conditionals-single-example.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-06-26 23:22:57.000000 dtschema-2023.6/test/schemas/good-example.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-26 23:22:57.000000 dtschema-2023.6/test/simple-bus-fail.dts
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-26 23:22:57.000000 dtschema-2023.6/test/simple-bus-pass.dts
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5664 2023-06-26 23:22:57.000000 dtschema-2023.6/test/test-dt-validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 23:23:10.406568 dtschema-2023.6/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1333 2023-06-26 23:22:57.000000 dtschema-2023.6/tools/dt-check-compatible
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2070 2023-06-26 23:22:57.000000 dtschema-2023.6/tools/dt-doc-validate
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2628 2023-06-26 23:22:57.000000 dtschema-2023.6/tools/dt-extract-example
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1916 2023-06-26 23:22:57.000000 dtschema-2023.6/tools/dt-extract-props
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1494 2023-06-26 23:22:57.000000 dtschema-2023.6/tools/dt-mk-schema
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6206 2023-06-26 23:22:57.000000 dtschema-2023.6/tools/dt-prop-populate
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5314 2023-06-26 23:22:57.000000 dtschema-2023.6/tools/dt-validate
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1321 2023-06-26 23:22:57.000000 dtschema-2023.6/tools/dtb2py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1225 2023-06-26 23:22:57.000000 dtschema-2023.6/tools/extract-compatibles
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2135 2023-06-26 23:22:57.000000 dtschema-2023.6/tools/yaml-format
+-rwxr-xr-x   0 runner    (1001) docker     (123)      766 2023-06-26 23:22:57.000000 dtschema-2023.6/tools/yaml2json
```

### Comparing `dtschema-2023.4/.github/workflows/ci.yml` & `dtschema-2023.6/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/.github/workflows/publish.yml` & `dtschema-2023.6/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/LICENSE.txt` & `dtschema-2023.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/PKG-INFO` & `dtschema-2023.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtschema
-Version: 2023.4
+Version: 2023.6
 Summary: DeviceTree validation schema and tools
 Home-page: https://github.com/devicetree-org/dt-schema
 Author: Rob Herring
 Author-email: robh@kernel.org
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `dtschema-2023.4/README.md` & `dtschema-2023.6/README.md`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/dtb.py` & `dtschema-2023.6/dtschema/dtb.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # SPDX-License-Identifier: BSD-2-Clause
 # Copyright 2021-2022 Arm Ltd.
 # Python library for Devicetree schema validation
 
 import sys
 import struct
-import pprint
 
 import libfdt
 from libfdt import QUIET_NOTFOUND
 
 import dtschema
 
 u8 = struct.Struct('B')
@@ -63,27 +62,27 @@
             stride = d
     if match == 1:
         return stride
 
     return 0
 
 
-def prop_value(nodename, p):
+def prop_value(validator, nodename, p):
     # First, check for a boolean type
     if not len(p):
         return True
 
     dim = None
     data = bytes(p)
     fmt = None
 
     if nodename in {'__fixups__', 'aliases'}:
         return data[:-1].decode(encoding='ascii').split('\0')
 
-    prop_types = set(dtschema.property_get_type(p.name))
+    prop_types = set(validator.property_get_type(p.name))
     prop_types -= {'node'}
 
     # Filter out types impossible for the size of the property
     if len(prop_types) > 1:
         if len(p) > 4:
             prop_types -= {'int32', 'uint32'}
         else:
@@ -159,15 +158,15 @@
             type_struct = type_format['uint8']
         else:
             return data
         for i in type_struct.iter_unpack(data):
             val_int += [dtschema.sized_int(i[0], size=(type_struct.size * 8))]
 
     if 'matrix' in fmt or 'phandle-array' in fmt:
-        dim = dtschema.property_get_type_dim(p.name)
+        dim = validator.property_get_type_dim(p.name)
     if dim:
         if max(dim[1]) and dim[1][0] == dim[1][1]:
             stride = dim[1][1]
         elif max(dim[0]) and dim[0][0] == dim[0][1]:
             stride, rem = divmod(len(val_int), dim[0][1])
             if rem:
                 stride = len(val_int)
@@ -181,34 +180,34 @@
 
         #print(p.name, dim, stride)
         return [val_int[i:i+stride] for i in range(0, len(val_int), stride)]
 
     return [val_int]
 
 
-def node_props(fdt, nodename, offset):
+def node_props(validator, fdt, nodename, offset):
     props_dict = {}
     poffset = fdt.first_property_offset(offset, QUIET_NOTFOUND)
     while poffset >= 0:
         p = fdt.get_property_by_offset(poffset)
-        props_dict[p.name] = prop_value(nodename, p)
+        props_dict[p.name] = prop_value(validator, nodename, p)
 
         poffset = fdt.next_property_offset(poffset, QUIET_NOTFOUND)
 
     return props_dict
 
 
 phandles = {}
 phandle_loc = []
 
 
-def process_fixups(fdt, nodename, offset):
+def process_fixups(validator, fdt, nodename, offset):
     if nodename != '__fixups__':
         return
-    props = node_props(fdt, nodename, offset)
+    props = node_props(validator, fdt, nodename, offset)
     global phandle_loc
     phandle_loc += [s for l in props.values() for s in l]
 
 
 def process_local_fixups(fdt, nodename, path, offset):
     global phandle_loc
 
@@ -228,33 +227,33 @@
     while offset >= 0:
         nodename = fdt.get_name(offset)
         process_local_fixups(fdt, nodename, path, offset)
 
         offset = fdt.next_subnode(offset, QUIET_NOTFOUND)
 
 
-def fdt_scan_node(fdt, nodename, offset):
+def fdt_scan_node(validator, fdt, nodename, offset):
     if nodename == '__fixups__':
-        process_fixups(fdt, nodename, offset)
+        process_fixups(validator, fdt, nodename, offset)
         return
     if nodename == '__local_fixups__':
         process_local_fixups(fdt, '', '', offset)
         return
     if nodename.startswith('__'):
         return
 
-    node_dict = node_props(fdt, nodename, offset)
+    node_dict = node_props(validator, fdt, nodename, offset)
     if 'phandle' in node_dict:
         #print('phandle', node_dict['phandle'])
         phandles[node_dict['phandle'][0][0]] = node_dict
 
     offset = fdt.first_subnode(offset, QUIET_NOTFOUND)
     while offset >= 0:
         nodename = fdt.get_name(offset)
-        node = fdt_scan_node(fdt, nodename, offset)
+        node = fdt_scan_node(validator, fdt, nodename, offset)
         if node is not None:
             node_dict[nodename] = node
 
         offset = fdt.next_subnode(offset, QUIET_NOTFOUND)
 
     return node_dict
 
@@ -314,22 +313,22 @@
         return 0
 
     node = phandles[phandle]
 
     return _get_cells_size(node, cellname) + 1
 
 
-def fixup_phandles(dt, path=''):
+def fixup_phandles(validator, dt, path=''):
     for k, v in dt.items():
         if isinstance(v, dict):
-            fixup_phandles(v, path=path + '/' + k)
+            fixup_phandles(validator, v, path=path + '/' + k)
             continue
-        elif not {'phandle-array'} & set(dtschema.property_get_type(k)):
+        elif not {'phandle-array'} & set(validator.property_get_type(k)):
             continue
-        elif dtschema.property_has_fixed_dimensions(k):
+        elif validator.property_has_fixed_dimensions(k):
             continue
         elif not isinstance(v, list) or (len(v) > 1 or not isinstance(v[0], list)):
             # Not a matrix or already split, nothing to do
             continue
         elif k in phandle_args:
             cellname = phandle_args[k]
         elif k.endswith('s') and 'gpio' not in k:
@@ -470,21 +469,21 @@
             dt[k] = []
             val = v[0]
             while i < len(val):
                 dt[k] += [val[i:i + ac + child_cells]]
                 i += ac + child_cells
 
 
-def fdt_unflatten(dtb):
+def fdt_unflatten(validator, dtb):
     fdt = libfdt.Fdt(dtb)
 
     offset = fdt.first_subnode(-1, QUIET_NOTFOUND)
-    dt = fdt_scan_node(fdt, '/', offset)
+    dt = fdt_scan_node(validator, fdt, '/', offset)
 
     #print(phandle_loc)
     fixup_gpios(dt)
     fixup_interrupts(dt, 1)
     fixup_addresses(dt, 2, 1)
-    fixup_phandles(dt)
+    fixup_phandles(validator, dt)
 
 #    pprint.pprint(dt, compact=True)
     return dt
```

### Comparing `dtschema-2023.4/dtschema/meta-schemas/base.yaml` & `dtschema-2023.6/dtschema/meta-schemas/string-array.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,60 +1,77 @@
 # SPDX-License-Identifier: BSD-2-Clause
 # Copyright 2018 Linaro Ltd.
-# Copyright 2018 Arm Ltd.
+# Copyright 2018-2019 Arm Ltd.
 %YAML 1.2
 ---
-$id: http://devicetree.org/meta-schemas/base.yaml#
+$id: http://devicetree.org/meta-schemas/string-array.yaml#
 $schema: https://json-schema.org/draft/2019-09/schema
-description: Metaschema for devicetree binding documentation
+#type: object
+
+if:
+  not:
+    required:
+      - minItems
+      - maxItems
+then:
+  properties:
+    items:
+      type: array
 
 allOf:
-  - $ref: http://json-schema.org/draft-07/schema#
-  - $ref: http://devicetree.org/meta-schemas/keywords.yaml#
+  - $ref: '#/all-properties'
 
-properties:
-  # listing all properties here to narrow the scope of what is allowed in
-  # devicetree schema files. This list can be relaxed in the future as we
-  # become more comfortable with the validation vocabulary.
-  # Also, being explicit about what properties are allowed helps to catch
-  # misspelled or unsupported tests.
-  $id:
-    pattern: 'http://devicetree.org/schemas/.*\.yaml#'
-  $schema:
-    enum:
-      - "http://devicetree.org/meta-schemas/core.yaml#"
-      - "http://devicetree.org/meta-schemas/base.yaml#"
-  title:
-    maxLength: 100
-  examples:
-    type: array
+all-properties:
+  properties:
+    description: {}
+    minItems:
+      minimum: 1
+    maxItems:
+      minimum: 1
     items:
+      oneOf:
+        - type: object
+          allOf:
+            - $ref: '#/all-properties'
+        - type: array
+          minItems: 1
+          items:
+            allOf:
+              - $ref: '#/all-properties'
+              - properties:
+                  enum: {}
+                  const: {}
+                  pattern: {}
+                additionalProperties: false
+    enum:
+      type: array
+      items:
+        type: string
+        pattern: '^[a-zA-Z0-9,.\-_ #+/]+$'
+    const:
       type: string
-
-  maintainers:
-    type: array
-    items:
+      pattern: '^[a-zA-Z0-9,.\-_ #+/]+$'
+    contains:
+      $ref: '#/all-properties'
+    default: {}
+    deprecated: {}
+    pattern:
       type: string
-      format: email
 
-  select:
-    description: '"select" must contain a valid json-schema'
+    oneOf:
+      type: array
+      items:
+        $ref: '#/all-properties'
     allOf:
-      - $ref: http://json-schema.org/draft-07/schema#
-      - oneOf:
-          - type: object
-            properties:
-              properties: true
-              required: true
-          - type: boolean
-
-propertyNames:
-  enum: [ $id, $schema, title, description, examples, required, allOf, anyOf, oneOf,
-          definitions, $defs, additionalProperties, dependencies, dependentRequired,
-          dependentSchemas, patternProperties, properties, not, if, then, else,
-          unevaluatedProperties, deprecated, maintainers, select, $ref ]
-
-required:
-  - $id
-  - $schema
-  - title
-  - maintainers
+      type: array
+      items:
+        $ref: '#/all-properties'
+    anyOf:
+      type: array
+      items:
+        $ref: '#/all-properties'
+    $ref: {}
+
+    additionalItems:
+      type: boolean
+
+  additionalProperties: false
```

### Comparing `dtschema-2023.4/dtschema/meta-schemas/cell.yaml` & `dtschema-2023.6/dtschema/meta-schemas/cell.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/meta-schemas/clocks.yaml` & `dtschema-2023.6/dtschema/meta-schemas/clocks.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/meta-schemas/core.yaml` & `dtschema-2023.6/dtschema/meta-schemas/core.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
       '^#.*-cells$':
         $ref: cell.yaml#/single
 
       '-supply$':
         propertyNames:
           enum: [ description, deprecated ]
 
-      '-(bits|-kBps|percent|bp|mhz|hz|sec|ms|us|ns|ps|mm|microamp(-hours)?|(micro-)?ohms|microwatt-hours|microvolt|(femto|pico)farads|(milli)?celsius|kelvin|kpascal)$':
+      '-(bits|-kBps|percent|bp|mhz|hz|sec|ms|us|ns|ps|mm|nanoamp|microamp(-hours)?|(micro-)?ohms|microwatt-hours|microvolt|(femto|pico)farads|(milli)?celsius|kelvin|kpascal)$':
         allOf:
           - $ref: cell.yaml#/array
           - description: Standard unit suffix properties don't need a type $ref
             propertyNames:
               not:
                 const: $ref
```

### Comparing `dtschema-2023.4/dtschema/meta-schemas/gpios.yaml` & `dtschema-2023.6/dtschema/meta-schemas/gpios.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/meta-schemas/interrupts.yaml` & `dtschema-2023.6/dtschema/meta-schemas/interrupts.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/meta-schemas/items.yaml` & `dtschema-2023.6/dtschema/meta-schemas/items.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/meta-schemas/keywords.yaml` & `dtschema-2023.6/dtschema/meta-schemas/keywords.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -99,14 +99,23 @@
   then:
     - if
   else:
     - if
     - then
 
 properties:
+  $defs:
+    propertyNames:
+      description: A json-schema keyword was found in $defs key.
+      not:
+        $ref: "#/definitions/json-schema-prop-names"
+    additionalProperties:
+      description: $defs entries must contain schemas
+      type: object
+      $ref: "#/definitions/sub-schemas"
   $ref:
     description:
       References must start with '/schemas' or be relative to current
       schema's path.
     pattern: '^(/schemas/|\.\./|#(/|$)|[a-zA-Z0-9]+)'
     not:
       pattern: '^https?://'
@@ -131,16 +140,22 @@
   dependentRequired:
     uniqueItems: true
   else:
     $ref: "#/definitions/sub-schemas"
   const:
     type: [ integer, string ]
   enum:
+    description: '"enum" must be an array of either integers or strings'
     type: array
     uniqueItems: true
+    oneOf:
+      - items:
+          type: integer
+      - items:
+          type: string
   if:
     $ref: "#/definitions/sub-schemas"
   items:
     oneOf:
       - type: object
         allOf:
           - $ref: "#/definitions/sub-schemas"
@@ -182,14 +197,15 @@
       allOf:
         - description: Expected a valid DT property name
           pattern:  "^[#$a-zA-Z][a-zA-Z0-9#,+\\-._@]{0,63}$"
         - description: A json-schema keyword was found instead of a DT property name.
           not:
             $ref: "#/definitions/json-schema-prop-names"
     additionalProperties:
+      type: [ object, boolean ]
       $ref: "#/definitions/sub-schemas"
   required:
     description: "'required' must be valid DT property or node names"
     type: array
     uniqueItems: true
     items:
       pattern: '^([a-zA-Z#][a-zA-Z0-9,+\-._@]{0,63}|\$nodename)$'
```

### Comparing `dtschema-2023.4/dtschema/meta-schemas/nodes.yaml` & `dtschema-2023.6/dtschema/meta-schemas/nodes.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/meta-schemas/vendor-props.yaml` & `dtschema-2023.6/dtschema/meta-schemas/vendor-props.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/schemas/aliases.yaml` & `dtschema-2023.6/dtschema/schemas/aliases.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/schemas/bootph.yaml` & `dtschema-2023.6/dtschema/schemas/bootph.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/schemas/bus/qemu,platform.yaml` & `dtschema-2023.6/dtschema/schemas/bus/qemu,platform.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/schemas/cache-controller.yaml` & `dtschema-2023.6/dtschema/schemas/cache-controller.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/schemas/cache.yaml` & `dtschema-2023.6/dtschema/schemas/cache.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/schemas/chosen.yaml` & `dtschema-2023.6/dtschema/schemas/chosen.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/schemas/clock/clock.yaml` & `dtschema-2023.6/dtschema/schemas/clock/clock.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/schemas/cpu.yaml` & `dtschema-2023.6/dtschema/schemas/cpu.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Copyright 2016,2017 Arm,Ltd.
 #
 %YAML 1.2
 ---
 $id: http://devicetree.org/schemas/cpu.yaml#
 $schema: http://devicetree.org/meta-schemas/base.yaml#
 
-title: Common cpu node binding
+title: CPU node common properties
 
 maintainers:
   - Devicetree Specification Mailing List <devicetree-spec@vger.kernel.org>
 
 description: |+
   In Devicetree data files, the layout of CPUs is described in the
   "cpus" node.  This node in turn contains a number of subnodes
@@ -41,18 +41,26 @@
   reg:
     description:
       Defines a unique CPU/thread ID for the CPU/threads represented
       by the CPU node.
 
   compatible: true
 
+  '#cooling-cells':
+    const: 2
+
   clock-frequency:
     description:
       Specifies the current clock speed of the CPU in Hertz.
 
+  clocks: true
+  clock-names: true
+
+  cpu-supply: true
+
   timebase-frequency:
     oneOf:
       - $ref: /schemas/types.yaml#/definitions/uint32
       - $ref: /schemas/types.yaml#/definitions/uint64
     minimum: 1
     description:
       Specifies the current frequency at which the timebase and the
@@ -89,27 +97,37 @@
 
   reservation-granule-size:
     $ref: /schemas/types.yaml#/definitions/uint32
     description:
       Specifies the reservation granule size supported by this processor
       in bytes.
 
+  numa-node-id: true
+
   mmu-type:
     $ref: /schemas/types.yaml#/definitions/string
     description:
       Specifies the CPU's MMU type.
 
+  operating-points-v2: true
+
   tlb-split:
     $ref: /schemas/types.yaml#/definitions/flag
     description:
       If present, specifies that the TLB has a split configuration, with
       separate TLBs for instructions and data.  If absent, specifies that
       the TLB has a unified configuration.  Required for a CPU with a
       TLB in a split configuration.
 
+  l2-cache:
+    oneOf:
+      - type: object
+      - $ref: /schemas/types.yaml#/definitions/phandle
+        deprecated: true
+
 patternProperties:
   "^(i-|d-|)tlb-(size|sets)$":
     $ref: /schemas/types.yaml#/definitions/uint32
     minimum: 1
 
 anyOf:
   - required:
```

### Comparing `dtschema-2023.4/dtschema/schemas/cpus.yaml` & `dtschema-2023.6/dtschema/schemas/cpus.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/schemas/dt-core.yaml` & `dtschema-2023.6/dtschema/schemas/dt-core.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 properties:
   $nodename:
     $ref: types.yaml#/definitions/string
   compatible:
     $ref: types.yaml#/definitions/string-array
     items:
       # Keep in sync with make_compatible_schema()
-      pattern: "^[a-zA-Z0-9][a-zA-Z0-9,+\\-._]+$"
+      pattern: "^[a-zA-Z0-9][a-zA-Z0-9,+\\-._/]+$"
   cpus:
     description:
       Phandles to CPU nodes associated with the referring node.
     oneOf:
       - type: object
       - $ref: types.yaml#/definitions/phandle-array
         items:
@@ -41,41 +41,42 @@
     $ref: types.yaml#/definitions/string-array
     description:
       The filename for a device's firmware file. It is typically a single
       entry, but some devices have multiple firmware files. It can also
       be just a stem name used to construct the full firmware filename(s).
   secure-status:
     $ref: types.yaml#/definitions/string
-    enum: [ okay, disabled, reserved ]
+    enum: [ okay, disabled, reserved, fail ]
   status:
-    $ref: types.yaml#/definitions/string
-    enum: [ okay, disabled, reserved ]
+    oneOf:
+      - type: object
+      - $ref: types.yaml#/definitions/string
+        enum: [ okay, disabled, reserved, fail ]
   phandle:
     $ref: types.yaml#/definitions/uint32
 
 patternProperties:
   "^#.*-cells$":
     $ref: types.yaml#/definitions/uint32
     maximum: 8
 
   ".*-names$":
     $ref: types.yaml#/definitions/non-unique-string-array
 
   ".*-supply$":
-    if:
-      not: { type: object }
-    then:
-      $ref: types.yaml#/definitions/phandle
+    oneOf:
+      - type: object
+      - $ref: types.yaml#/definitions/phandle
 
   # property and node namespace overlaps. Catch both here
   "^[a-zA-Z0-9][a-zA-Z0-9,+\\-._]{0,63}$":
     type: [object, array, boolean, 'null']
 
   # Anything with a '@' is definitely a node
-  "^[a-zA-Z][a-zA-Z0-9,+\\-._]{0,63}@[0-9a-fA-F]+(,[0-9a-fA-F]+)*$":
+  "^[a-zA-Z0-9][a-zA-Z0-9,+\\-._]{0,63}@[0-9a-fA-F]+(,[0-9a-fA-F]+)*$":
     type: object
 
   # Anything beginnning and ending with '__' is a generated node
   "^__.*__$":
     type: object
 
   # Anything with a '#' is single cell number
```

### Comparing `dtschema-2023.4/dtschema/schemas/gpio/gpio-consumer.yaml` & `dtschema-2023.6/dtschema/schemas/gpio/gpio-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/schemas/gpio/gpio-hog.yaml` & `dtschema-2023.6/dtschema/schemas/gpio/gpio-hog.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/schemas/gpio/gpio.yaml` & `dtschema-2023.6/dtschema/schemas/gpio/gpio.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/schemas/graph.yaml` & `dtschema-2023.6/dtschema/schemas/graph.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/schemas/hwlock/hwlock-consumer.yaml` & `dtschema-2023.6/dtschema/schemas/hwlock/hwlock-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/schemas/i2c/i2c-controller.yaml` & `dtschema-2023.6/dtschema/schemas/i2c/i2c-controller.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/schemas/iio/iio-consumer.yaml` & `dtschema-2023.6/dtschema/schemas/iio/iio-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/schemas/iio/iio.yaml` & `dtschema-2023.6/dtschema/schemas/iio/iio.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -26,14 +26,18 @@
   "#io-channel-cells":
     enum: [0, 1, 2]
     description: >
       Number of cells in an IIO specifier; Typically 0 for nodes
       with a single IIO output and 1 for nodes with multiple IIO outputs.
       A few unusual devices have a 2 level mapping.
 
+  label:
+    description:
+      Unique name to identify which IIO channel or device this is.
+
   mount-matrix:
     $ref: /schemas/types.yaml#/definitions/non-unique-string-array
     minItems: 9
     maxItems: 9
     description:
       3x3 matrix specifying the sensor orientation wrt to a reference plane.
```

### Comparing `dtschema-2023.4/dtschema/schemas/interrupt-controller.yaml` & `dtschema-2023.6/dtschema/schemas/interrupt-controller.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/schemas/interrupts.yaml` & `dtschema-2023.6/dtschema/schemas/interrupts.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/schemas/isa/isa-bridge.yaml` & `dtschema-2023.6/dtschema/schemas/isa/isa-bridge.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/schemas/isa/isa-bus.yaml` & `dtschema-2023.6/dtschema/schemas/isa/isa-bus.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/schemas/mbox/mbox-consumer.yaml` & `dtschema-2023.6/dtschema/schemas/mbox/mbox-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/schemas/memory.yaml` & `dtschema-2023.6/dtschema/schemas/memory.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/schemas/msi-consumer.yaml` & `dtschema-2023.6/dtschema/schemas/msi-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/schemas/opp/opp.yaml` & `dtschema-2023.6/dtschema/schemas/opp/opp.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/schemas/options/u-boot.yaml` & `dtschema-2023.6/dtschema/schemas/options/u-boot.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/schemas/options.yaml` & `dtschema-2023.6/dtschema/schemas/options.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/schemas/pci/pci-bus.yaml` & `dtschema-2023.6/dtschema/schemas/pci/pci-bus.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/schemas/pci/pci-iommu.yaml` & `dtschema-2023.6/dtschema/schemas/pci/pci-iommu.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/schemas/phy/phy-consumer.yaml` & `dtschema-2023.6/dtschema/schemas/phy/phy-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/schemas/phy/phy-provider.yaml` & `dtschema-2023.6/dtschema/schemas/phy/phy-provider.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/schemas/pinctrl/pinctrl-consumer.yaml` & `dtschema-2023.6/dtschema/schemas/pinctrl/pinctrl-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/schemas/power-domain/power-domain-consumer.yaml` & `dtschema-2023.6/dtschema/schemas/power-domain/power-domain-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/schemas/property-units.yaml` & `dtschema-2023.6/dtschema/schemas/property-units.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/schemas/pwm/pwm-consumer.yaml` & `dtschema-2023.6/dtschema/schemas/pwm/pwm-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/schemas/reg.yaml` & `dtschema-2023.6/dtschema/schemas/reg.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/schemas/reset/reset.yaml` & `dtschema-2023.6/dtschema/schemas/reset/reset.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/schemas/root-node.yaml` & `dtschema-2023.6/dtschema/schemas/root-node.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/schemas/simple-bus.yaml` & `dtschema-2023.6/dtschema/schemas/simple-bus.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema/schemas/types.yaml` & `dtschema-2023.6/dtschema/schemas/types.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/dtschema.egg-info/PKG-INFO` & `dtschema-2023.6/dtschema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtschema
-Version: 2023.4
+Version: 2023.6
 Summary: DeviceTree validation schema and tools
 Home-page: https://github.com/devicetree-org/dt-schema
 Author: Rob Herring
 Author-email: robh@kernel.org
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `dtschema-2023.4/dtschema.egg-info/SOURCES.txt` & `dtschema-2023.6/dtschema.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 example-schema.yaml
 setup.py
 .github/workflows/ci.yml
 .github/workflows/publish.yml
 dtschema/.gitignore
 dtschema/__init__.py
 dtschema/dtb.py
+dtschema/fixups.py
 dtschema/lib.py
+dtschema/schema.py
+dtschema/validator.py
 dtschema/version.py
 dtschema.egg-info/PKG-INFO
 dtschema.egg-info/SOURCES.txt
 dtschema.egg-info/dependency_links.txt
 dtschema.egg-info/requires.txt
 dtschema.egg-info/top_level.txt
 dtschema/meta-schemas/base.yaml
```

### Comparing `dtschema-2023.4/example-schema.yaml` & `dtschema-2023.6/example-schema.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/setup.py` & `dtschema-2023.6/setup.py`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/test/child-node-fail.dts` & `dtschema-2023.6/test/child-node-fail.dts`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/test/child-node.dts` & `dtschema-2023.6/test/child-node.dts`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/test/conditionals-allof-fail.dts` & `dtschema-2023.6/test/conditionals-allof-fail.dts`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/test/conditionals-allof-pass.dts` & `dtschema-2023.6/test/conditionals-allof-pass.dts`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/test/conditionals-single-fail.dts` & `dtschema-2023.6/test/conditionals-single-fail.dts`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/test/device-fail.dts` & `dtschema-2023.6/test/device-fail.dts`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/test/device.dts` & `dtschema-2023.6/test/device.dts`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/test/schemas/bad-example.yaml` & `dtschema-2023.6/test/schemas/bad-example.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/test/schemas/child-node-example.yaml` & `dtschema-2023.6/test/schemas/child-node-example.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/test/schemas/conditionals-allof-example.yaml` & `dtschema-2023.6/test/schemas/conditionals-allof-example.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/test/schemas/conditionals-single-example.yaml` & `dtschema-2023.6/test/schemas/conditionals-single-example.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/test/schemas/good-example.yaml` & `dtschema-2023.6/test/schemas/good-example.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/test/simple-bus-pass.dts` & `dtschema-2023.6/test/simple-bus-pass.dts`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/test/test-dt-validate.py` & `dtschema-2023.6/test/test-dt-validate.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,144 +6,135 @@
 #
 # SPDX-License-Identifier: BSD-2-Clause
 #
 # Testcases are executed by running 'make test' from the top level directory of this repo.
 
 import unittest
 import os
+import copy
 import glob
 import sys
 import subprocess
 import tempfile
 
 basedir = os.path.dirname(__file__)
 import jsonschema
+import ruamel.yaml
 import dtschema
 
 dtschema_dir = os.path.dirname(dtschema.__file__)
 
+yaml = ruamel.yaml.YAML(typ='safe')
+
+def load(filename):
+    with open(filename, 'r', encoding='utf-8') as f:
+        return yaml.load(f.read())
+
 class TestDTMetaSchema(unittest.TestCase):
     def setUp(self):
-        self.schema = dtschema.load(os.path.join(basedir, 'schemas/good-example.yaml'))
-        self.bad_schema = dtschema.load(os.path.join(basedir, 'schemas/bad-example.yaml'))
+        self.schema = dtschema.DTSchema(os.path.join(basedir, 'schemas/good-example.yaml'))
+        self.bad_schema = dtschema.DTSchema(os.path.join(basedir, 'schemas/bad-example.yaml'))
 
     def test_all_metaschema_valid(self):
         '''The metaschema must all be a valid Draft2019-09 schema'''
         for filename in glob.iglob(os.path.join(dtschema_dir, 'meta-schemas/**/*.yaml'), recursive=True):
             with self.subTest(schema=filename):
-                schema = dtschema.load_schema(filename)
+                schema = load(filename)
                 jsonschema.Draft201909Validator.check_schema(schema)
 
     def test_required_properties(self):
-        dtschema.DTValidator.check_schema(self.schema)
+        self.schema.is_valid(strict=True)
 
     def test_required_property_missing(self):
         for key in self.schema.keys():
             if key in ['$schema', 'properties', 'required', 'description', 'examples', 'additionalProperties']:
                 continue
             with self.subTest(k=key):
-                schema_tmp = self.schema.copy()
+                schema_tmp = copy.deepcopy(self.schema)
                 del schema_tmp[key]
-                self.assertRaises(jsonschema.SchemaError, dtschema.DTValidator.check_schema, schema_tmp)
+                self.assertRaises(jsonschema.SchemaError, schema_tmp.is_valid, strict=True)
 
     def test_bad_schema(self):
         '''bad-example.yaml is all bad. There is no condition where it should pass validation'''
-        self.assertRaises(jsonschema.SchemaError, dtschema.DTValidator.check_schema, self.bad_schema)
+        self.assertRaises(jsonschema.SchemaError, self.bad_schema.is_valid, strict=True)
 
     def test_bad_properties(self):
         for key in self.bad_schema.keys():
             if key in ['$schema', 'properties']:
                 continue
 
             with self.subTest(k=key):
-                schema_tmp = self.schema.copy()
+                schema_tmp = copy.deepcopy(self.schema)
                 schema_tmp[key] = self.bad_schema[key]
-                self.assertRaises(jsonschema.SchemaError, dtschema.DTValidator.check_schema, schema_tmp)
+                self.assertRaises(jsonschema.SchemaError, schema_tmp.is_valid, strict=True)
 
         bad_props = self.bad_schema['properties']
-        schema_tmp = self.schema.copy()
+        schema_tmp = copy.deepcopy(self.schema)
         for key in bad_props.keys():
             with self.subTest(k="properties/"+key):
                 schema_tmp['properties'] = self.schema['properties'].copy()
                 schema_tmp['properties'][key] = bad_props[key]
-                self.assertRaises(jsonschema.SchemaError, dtschema.DTValidator.check_schema, schema_tmp)
+                self.assertRaises(jsonschema.SchemaError, schema_tmp.is_valid, strict=True)
 
 class TestDTSchema(unittest.TestCase):
     def test_binding_schemas_valid(self):
         '''Test that all schema files under ./dtschema/schemas/ validate against the DT metaschema'''
         for filename in glob.iglob(os.path.join(dtschema_dir, 'schemas/**/*.yaml'), recursive=True):
             with self.subTest(schema=filename):
-                schema = dtschema.load_schema(filename)
-                dtschema.DTValidator.check_schema(schema)
+                dtschema.DTSchema(filename).is_valid(strict=True)
 
     def test_binding_schemas_id_is_unique(self):
         '''Test that all schema files under ./dtschema/schemas/ validate against the DT metaschema'''
         ids = []
         for filename in glob.iglob(os.path.join(dtschema_dir, 'schemas/**/*.yaml'), recursive=True):
             with self.subTest(schema=filename):
-                schema = dtschema.load_schema(filename)
+                schema = load(filename)
                 self.assertEqual(ids.count(schema['$id']), 0)
                 ids.append(schema['$id'])
 
     def test_binding_schemas_valid_draft7(self):
         '''Test that all schema files under ./dtschema/schemas/ validate against the Draft7 metaschema
         The DT Metaschema is supposed to force all schemas to be valid against
         Draft7. This test makes absolutely sure that they are.
         '''
         for filename in glob.iglob(os.path.join(dtschema_dir, 'schemas/**/*.yaml'), recursive=True):
             with self.subTest(schema=filename):
-                schema = dtschema.load_schema(filename)
+                schema = load(filename)
                 jsonschema.Draft7Validator.check_schema(schema)
 
 
 class TestDTValidate(unittest.TestCase):
     def setUp(self):
-        self.schemas = list()
-
-        self.schemas = dtschema.set_schemas([ os.path.join(os.path.abspath(basedir), "schemas/")])
-
-        for schema in self.schemas.values():
-            schema["$select_validator"] = dtschema.DTValidator(schema['select'])
+        self.validator = dtschema.DTValidator([ os.path.join(os.path.abspath(basedir), "schemas/")])
 
-    def check_node(self, nodename, node, fail):
+    def check_node(self, nodename, node):
         if nodename == "/" or nodename.startswith('__'):
             return
 
         node['$nodename'] = [ nodename ]
-        node_matched = True
-        if fail:
-            node_matched = False
-            with self.assertRaises(jsonschema.ValidationError, msg=nodename):
-                for schema in self.schemas.values():
-                    if schema['$select_validator'].is_valid(node):
-                        node_matched = True
-                        dtschema.DTValidator(schema).validate(node)
-        else:
-            node_matched = False
-            for schema in self.schemas.values():
-                if schema['$select_validator'].is_valid(node):
-                    node_matched = True
-                    self.assertIsNone(dtschema.DTValidator(schema).validate(node))
+        self.validator.validate(node)
 
-        self.assertTrue(node_matched, msg=nodename)
-
-    def check_subtree(self, nodename, subtree, fail):
-        self.check_node(nodename, subtree, fail)
+    def check_subtree(self, nodename, subtree):
+        self.check_node(nodename, subtree)
         for name,value in subtree.items():
             if isinstance(value, dict):
-                self.check_subtree(name, value, fail)
+                self.check_subtree(name, value)
 
     def test_dtb_validation(self):
         '''Test that all DT files under ./test/ validate against the DT schema (DTB)'''
         for filename in glob.iglob('test/*.dts'):
             with self.subTest(schema=filename):
                 expect_fail = "-fail" in filename
                 res = subprocess.run(['dtc', '-Odtb', filename], capture_output=True)
-                testtree = dtschema.dtb.fdt_unflatten(res.stdout)
+                testtree = self.validator.decode_dtb(res.stdout)
                 self.assertEqual(res.returncode, 0, msg='dtc failed:\n' + res.stderr.decode())
-                for name, value in testtree.items():
-                    if isinstance(value, dict):
-                        self.check_node(name, value, expect_fail)
+
+                if expect_fail:
+                    with self.assertRaises(jsonschema.ValidationError):
+                        self.check_subtree('/', testtree[0])
+                else:
+                    self.assertIsNone(self.check_subtree('/', testtree[0]))
+
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `dtschema-2023.4/tools/dt-check-compatible` & `dtschema-2023.6/tools/dt-check-compatible`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,13 @@
                     action="version", version=dtschema.__version__)
     ap.add_argument('-s', '--schema', required=True, help="path to processed schema file or schema directory")
     args = ap.parse_args()
 
     if args.schema != "" and not os.path.exists(args.schema):
         exit(-1)
 
-    dtschema.set_schemas([args.schema])
-
-    undoc_compats = dtschema.get_undocumented_compatibles(args.compatible_str)
+    undoc_compats = dtschema.DTValidator([args.schema]).get_undocumented_compatibles(args.compatible_str)
 
     if args.invert_match:
         print(*undoc_compats, sep="\n")
     else:
         print(*set(args.compatible_str).difference(undoc_compats), sep="\n")
```

### Comparing `dtschema-2023.4/tools/dt-doc-validate` & `dtschema-2023.6/tools/dt-doc-validate`

 * *Files 13% similar despite different names*

```diff
@@ -18,26 +18,30 @@
 import glob
 
 line_number = False
 
 def check_doc(filename):
     ret = 0
     try:
-        testtree = dtschema.load(filename, line_number=line_number)
+        dtsch = dtschema.DTSchema(filename, line_numbers=line_number)
     except ruamel.yaml.YAMLError as exc:
         print(filename + ":" + str(exc.problem_mark.line + 1) + ":" +
               str(exc.problem_mark.column + 1) + ":", exc.problem, file=sys.stderr)
         return 1
 
-    for error in sorted(dtschema.DTValidator.iter_schema_errors(testtree), key=lambda e: e.linecol):
-        print(dtschema.format_error(filename, error, verbose=args.verbose), file=sys.stderr)
-        ret = 1
+    try:
+        for error in sorted(dtsch.iter_errors(), key=lambda e: e.linecol):
+            print(dtschema.format_error(filename, error, verbose=args.verbose), file=sys.stderr)
+            ret = 1
+    except:
+        raise
+        print(filename + ': error checking schema file', file=sys.stderr)
+        return 1
 
-    dtschema.DTValidator.check_schema_refs(filename, testtree)
-    dtschema.DTValidator.check_quotes(filename + ":", testtree)
+    dtsch.check_schema_refs()
 
     return ret
 
 if __name__ == "__main__":
     ap = argparse.ArgumentParser(fromfile_prefix_chars='@',
         epilog='Arguments can also be passed in a file prefixed with a "@" character.')
     ap.add_argument("yamldt", nargs='*', type=str,
@@ -47,17 +51,14 @@
     ap.add_argument('-u', '--url-path', help="Additional search path for references")
     ap.add_argument('-V', '--version', help="Print version number",
                     action="version", version=dtschema.__version__)
     args = ap.parse_args()
 
     line_number=args.line_number
 
-    if args.url_path:
-        dtschema.add_schema_path(args.url_path)
-
     ret = 0
     for f in args.yamldt:
         if os.path.isdir(f):
             for filename in glob.iglob(f + "/**/*.yaml", recursive=True):
                 ret |= check_doc(filename)
         else:
             ret |= check_doc(f)
```

### Comparing `dtschema-2023.4/tools/dt-extract-example` & `dtschema-2023.6/tools/dt-extract-example`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/tools/dt-extract-props` & `dtschema-2023.6/tools/dt-extract-props`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,16 @@
                     help="preparsed schema file or list of additional schema files/directories")
     ap.add_argument('-d', '--duplicates', help="Only output properties with more than one type", action="store_true")
     ap.add_argument('-v', '--verbose', help="Additional search path for references", action="store_true")
     ap.add_argument('-V', '--version', help="Print version number",
                     action="version", version=dtschema.__version__)
     args = ap.parse_args()
 
-    dtschema.set_schemas(args.schema_files)
-    props = dtschema.extract_types()
+    dtval = dtschema.DTValidator(args.schema_files)
+    props = dtval.property_get_all()
 
     if args.duplicates:
         tmp_props = {}
         for k,v in props.items():
             if len(v) > 1:
                 tmp_props[k] = v
```

### Comparing `dtschema-2023.4/tools/dt-mk-schema` & `dtschema-2023.6/tools/dt-mk-schema`

 * *Files 14% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     ap.add_argument("schemas", nargs='*', type=str,
                     help="Names of directories, or YAML encoded schema files")
     ap.add_argument('-u', '--useronly', help="Only process user schemas", action="store_true")
     ap.add_argument('-V', '--version', help="Print version number",
                     action="version", version=dtschema.__version__)
     args = ap.parse_args()
 
-    schemas = dtschema.set_schemas(args.schemas, core_schema=(not args.useronly))
+    schemas = dtschema.DTValidator(args.schemas).schemas
     if not schemas:
         exit(-1)
 
     if args.outfile:
         f = open(args.outfile, 'w', encoding='utf-8')
     else:
         f = sys.stdout
```

### Comparing `dtschema-2023.4/tools/dt-prop-populate` & `dtschema-2023.6/tools/dt-prop-populate`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/tools/dt-validate` & `dtschema-2023.6/tools/dt-validate`

 * *Files 21% similar despite different names*

```diff
@@ -23,72 +23,58 @@
 match_schema_file = None
 
 class schema_group():
     def __init__(self, schema_file=""):
         if schema_file != "" and not os.path.exists(schema_file):
             exit(-1)
 
-        self.schemas = dtschema.set_schemas([schema_file])
+        self.validator = dtschema.DTValidator([schema_file])
 
     def check_node(self, tree, node, disabled, nodename, fullname, filename):
         # Hack to save some time validating examples
         if 'example-0' in node or 'example-' in nodename:
             return
 
         node['$nodename'] = [ nodename ]
-        node_matched = False
-        matched_schemas = []
-        for schema in self.schemas.values():
-            if '$select_validator' in schema and schema['$select_validator'].is_valid(node):
-                # We have a match if a conditional schema is selected
-                if schema['select'] != True:
-                    matched_schemas.append(schema['$id'])
-                    node_matched = True
-                try:
-                    for error in dtschema.DTValidator(schema).iter_errors(node):
-
-                        # Disabled nodes might not have all the required
-                        # properties filled in, such as a regulator or a
-                        # GPIO meant to be filled at the DTS level on
-                        # boards using that particular node. Thus, if the
-                        # node is marked as disabled, let's just ignore
-                        # any error message reporting a missing property.
-                        if disabled or (isinstance(error.instance, dict) and \
-                           'status' in error.instance and \
-                           'disabled' in error.instance['status']):
-                            if {'required', 'unevaluatedProperties'} & set(error.schema_path):
-                                continue
-                            elif error.context:
-                                found = False
-                                for e in error.context:
-                                    if {'required', 'unevaluatedProperties'} & set(e.schema_path):
-                                        found = True
-                                        break
-                                if found:
-                                    continue
-
-                        if schema['$id'] == 'generated-compatibles':
-                            if show_unmatched < 1:
-                                continue
-                            print("%s: %s: failed to match any schema with compatible: %s" %
-                                  (filename, fullname, node['compatible']), file=sys.stderr)
-                            continue
 
-                        print(dtschema.format_error(filename, error, nodename=nodename, verbose=verbose) +
-                            '\n\tFrom schema: ' + schema['$filename'],
-                            file=sys.stderr)
-                except RecursionError as e:
-                    print(ap.prog + ": recursion error: Check for prior errors in a referenced schema", file=sys.stderr)
-
-        if show_matched and matched_schemas:
-            print("%s: %s: matched on schema(s)\n\t" % (filename, fullname) +
-                '\n\t'.join(matched_schemas), file=sys.stderr)
+        try:
+            for error in self.validator.iter_errors(node, filter=match_schema_file):
+
+                # Disabled nodes might not have all the required
+                # properties filled in, such as a regulator or a
+                # GPIO meant to be filled at the DTS level on
+                # boards using that particular node. Thus, if the
+                # node is marked as disabled, let's just ignore
+                # any error message reporting a missing property.
+                if disabled or (isinstance(error.instance, dict) and \
+                    'status' in error.instance and \
+                    'disabled' in error.instance['status']):
+
+                    if {'required', 'unevaluatedProperties'} & set(error.schema_path):
+                        continue
+                    elif error.context:
+                        found = False
+                        for e in error.context:
+                            if {'required', 'unevaluatedProperties'} & set(e.schema_path):
+                                found = True
+                                break
+                        if found:
+                            continue
 
-        if show_unmatched >= 2 and not node_matched:
-            print("%s: %s: failed to match any schema" % (filename, fullname), file=sys.stderr)
+                if error.schema_file == 'generated-compatibles':
+                    if not show_unmatched:
+                        continue
+                    print(f"{filename}: {fullname}: failed to match any schema with compatible: {node['compatible']}",
+                          file=sys.stderr)
+                    continue
+
+                print(dtschema.format_error(filename, error, nodename=nodename, verbose=verbose),
+                    file=sys.stderr)
+        except RecursionError as e:
+            print(ap.prog + ": recursion error: Check for prior errors in a referenced schema", file=sys.stderr)
 
     def check_subtree(self, tree, subtree, disabled, nodename, fullname, filename):
         if nodename.startswith('__'):
             return
 
         try:
             disabled = ('disabled' in subtree['status'])
@@ -98,70 +84,57 @@
         self.check_node(tree, subtree, disabled, nodename, fullname, filename)
         if fullname != "/":
             fullname += "/"
         for name,value in subtree.items():
             if isinstance(value, dict):
                 self.check_subtree(tree, value, disabled, name, fullname + name, filename)
 
-    def check_trees(self, filename, dt):
+    def check_dtb(self, filename):
         """Check the given DT against all schemas"""
-
-        for schema in self.schemas.values():
-            if match_schema_file and match_schema_file not in schema['$filename']:
-                continue
-            schema["$select_validator"] = dtschema.DTValidator(schema['select'])
-
+        with open(filename, 'rb') as f:
+            dt = sg.validator.decode_dtb(f.read())
         for subtree in dt:
             self.check_subtree(dt, subtree, False, "/", "/", filename)
 
 if __name__ == "__main__":
     ap = argparse.ArgumentParser(fromfile_prefix_chars='@',
         epilog='Arguments can also be passed in a file prefixed with a "@" character.')
     ap.add_argument("dtbs", nargs='*',
                     help="Filename or directory of devicetree DTB input file(s)")
     ap.add_argument('-s', '--schema', help="preparsed schema file or path to schema files")
     ap.add_argument('-p', '--preparse', help="preparsed schema file (deprecated, use '-s')")
     ap.add_argument('-l', '--limit', help="limit validation to schema files matching substring")
-    ap.add_argument('-m', '--show-unmatched', default=0,
-        help="Print out nodes which don't match any schema.\n" \
-             "Once for only nodes with 'compatible'\n" \
-             "Twice for all nodes", action="count")
-    ap.add_argument('-M', '--show-matched',
-        help="Print out matching schema for each node", action="store_true")
+    ap.add_argument('-m', '--show-unmatched',
+        help="Print out node 'compatible' strings which don't match any schema.",
+        action="store_true")
     ap.add_argument('-n', '--line-number', help="Obsolete", action="store_true")
     ap.add_argument('-v', '--verbose', help="verbose mode", action="store_true")
     ap.add_argument('-u', '--url-path', help="Additional search path for references")
     ap.add_argument('-V', '--version', help="Print version number",
                     action="version", version=dtschema.__version__)
     args = ap.parse_args()
 
     verbose = args.verbose
     show_unmatched = args.show_unmatched
-    show_matched = args.show_matched
     match_schema_file = args.limit
 
-    if args.url_path:
-        dtschema.add_schema_path(args.url_path)
-
     if args.preparse:
         sg = schema_group(args.preparse)
     elif args.schema:
         sg = schema_group(args.schema)
     else:
         sg = schema_group()
 
     for d in args.dtbs:
         if not os.path.isdir(d):
             continue
         for filename in glob.iglob(d + "/**/*.dtb", recursive=True):
-            testtree = dtschema.load(filename)
             if verbose:
                 print("Check:  " + filename)
-            sg.check_trees(filename, testtree)
+            sg.check_dtb(filename)
 
     for filename in args.dtbs:
         if not os.path.isfile(filename):
             continue
-        testtree = dtschema.load(filename)
         if verbose:
             print("Check:  " + filename)
-        sg.check_trees(filename, testtree)
+        sg.check_dtb(filename)
```

### Comparing `dtschema-2023.4/tools/dtb2py` & `dtschema-2023.6/tools/dtb2py`

 * *Files 18% similar despite different names*

```diff
@@ -22,17 +22,17 @@
     if not os.path.isfile(args.dtbfile):
         exit(1)
 
     if args.schema:
         schemas = [args.schema]
     else:
         schemas = []
-    dtschema.set_schemas(schemas)
 
-    dt = dtschema.load(args.dtbfile)
+    with open(args.dtbfile, 'rb') as f:
+        dt = dtschema.DTValidator(schemas).decode_dtb(f.read())
 
     try:
         pprint.pprint(dt, compact=True)
         # flush output here to force SIGPIPE to be triggered
         # while inside this try block.
         sys.stdout.flush()
     except BrokenPipeError:
```

### Comparing `dtschema-2023.4/tools/extract-compatibles` & `dtschema-2023.6/tools/extract-compatibles`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/tools/yaml-format` & `dtschema-2023.6/tools/yaml-format`

 * *Files identical despite different names*

### Comparing `dtschema-2023.4/tools/yaml2json` & `dtschema-2023.6/tools/yaml2json`

 * *Files identical despite different names*


Shell scripts for toggling battery conservation mode on a Lenovo Yoga -laptop running Linux.

Turning on battery conservation mode stops charging the laptop battery at ~80%, prolonging its lifespan.

Scripts write to /sys/bus/platform/drivers/ideapad_acpi/VPC2004:00/conservation_mode, where a sole _1_ stands for conservation mode on, and _0_ for off. Elevated access rights are needed as the file is write-protected.

Written for and tested on a Lenovo Yoga Pro 7 14APH8 with Fedora 38-41 & KDE, but might also work on other Lenovo laptops and distros.

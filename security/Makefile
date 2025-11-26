#
# Makefile for the kernel security code
#

# hanya keys tetap aktif kalau CONFIG_KEYS=y
obj-$(CONFIG_KEYS) += keys/

# always enable default capabilities
obj-y += commoncap.o
obj-$(CONFIG_MMU) += min_addr.o

# Object file lists
obj-$(CONFIG_SECURITY) += security.o
obj-$(CONFIG_SECURITYFS) += inode.o
obj-$(CONFIG_AUDIT) += lsm_audit.o
obj-$(CONFIG_CGROUP_DEVICE) += device_cgroup.o

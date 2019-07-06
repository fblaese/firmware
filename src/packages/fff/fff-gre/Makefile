include $(TOPDIR)/rules.mk

PKG_NAME:=fff-gre
PKG_VERSION:=1
PKG_RELEASE:=1

PKG_BUILD_DIR:=$(BUILD_DIR)/fff-gre

include $(INCLUDE_DIR)/package.mk

define Package/fff-gre
	SECTION:=base
	CATEGORY:=Freifunk
	TITLE:=Freifunk-Franken gre
	URL:=https://www.freifunk-franken.de
	DEPENDS:=+gre \
			 +@PACKAGE_grev4 \
			 +@PACKAGE_grev6 \
			 +fff-network
endef

define Package/fff-gre/description
	This is the Freifunk Franken Firmware gre package.
	This package provides configuration scripts for gre tunnels.
endef

define Build/Prepare
	echo "all: " > $(PKG_BUILD_DIR)/Makefile
endef

define Build/Configure
	# nothing
endef

define Build/Compile
	# nothing
endef

define Package/fff-gre/install
	$(CP) ./files/* $(1)/
endef

$(eval $(call BuildPackage,fff-gre))

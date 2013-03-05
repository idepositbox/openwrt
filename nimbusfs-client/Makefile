#
# Copyright (C) 2013 iDepositBox
#
# See http://idepositbox.com for more details on copyright
# 
#
include $(TOPDIR)/rules.mk

PKG_NAME:=nimbusfs-client
PKG_VERSION:=master
PKG_RELEASE:=0

PKG_SOURCE_URL:= https://nodeload.github.com/fabregas/nimbusfs-client/tar.gz/
PKG_SOURCE:=master
PKG_CAT:=zcat
PKG_INSTALL:=1

include $(INCLUDE_DIR)/package.mk

define Package/nimbusfs-client
  SECTION:=admin
  CATEGORY:=Administration
  DEPENDS:=+python +python-crypto
  TITLE:=iDepositBox cloud client
  MAINTAINER:=dev-team@idepositbox.com
  URL:=http://idepositbox.com
endef

define Package/nimbusfs-client/description
	iDepositBox client
endef

#define Package/nimbusfs-client/conffiles
#endef

define Build/Configure
endef

define Build/Compile
endef

define Build/Install
endef

define Package/nimbusfs-client/install
	$(INSTALL_DIR) $(1)/opt/idepositbox
	$(CP) $(PKG_BUILD_DIR)/{bin,id_client,nimbus_client} $(1)/opt/idepositbox
endef

$(eval $(call BuildPackage,nimbusfs-client))

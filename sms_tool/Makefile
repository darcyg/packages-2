include $(TOPDIR)/rules.mk

PKG_NAME:=sms_tool
PKG_RELEASE:=1

PKG_SOURCE_URL:=https://github.com/obsy/sms_tool
PKG_SOURCE_PROTO:=git
PKG_SOURCE_DATE:=2017-10-05
PKG_SOURCE_VERSION:=4fc8a661a7e5310edf5a13022afd0f57f5a603e4

include $(INCLUDE_DIR)/package.mk

define Package/sms_tool
  SECTION:=utils
  CATEGORY:=Utilities
  TITLE:=sms tool
  URL:=https://github.com/obsy/sms_tool
endef

define Package/sms_tool/description
	SMS Tool for Various of 3G Modems
endef

define Package/sms_tool/install
	$(INSTALL_DIR) $(1)/usr/bin
	$(INSTALL_BIN) $(PKG_BUILD_DIR)/sms_tool $(1)/usr/bin/
endef

$(eval $(call BuildPackage,sms_tool))

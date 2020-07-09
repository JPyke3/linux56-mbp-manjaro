# Based on the file created for Arch Linux by:
# Tobias Powalowski <tpowa@archlinux.org>
# Thomas Baechler <thomas@archlinux.org>

# Maintainer: Philip Müller (x86_64) <philm@manjaro.org>
# Maintainer: Jonathon Fernyhough (i686) <jonathon@manjaro.org>
# Contributor: Helmut Stult <helmut[at]manjaro[dot]org>

pkgbase=linux56-mbp
pkgname=('linux56-mbp' 'linux56-mbp-headers' 'linux56-mbp-docs')
_kernelname=-MANJARO-mbp
_basekernel=5.6
_basever=56
_aufs=20200518
pkgver=5.6.19
pkgrel=2
arch=('x86_64')
url="http://www.kernel.org/"
license=('GPL2')
makedepends=('xmlto' 'docbook-xsl' 'kmod' 'inetutils' 'bc' 'elfutils' 'git')
options=('!strip')
source=("https://www.kernel.org/pub/linux/kernel/v5.x/linux-${_basekernel}.tar.xz"
        "https://www.kernel.org/pub/linux/kernel/v5.x/patch-${pkgver}.xz"
        # the main kernel config files
        'config.x86_64' 'config' 'config.aufs'
        # AUFS Patches
        "aufs5.6-${_aufs}.patch"
        'aufs5-base.patch'
        'aufs5-kbuild.patch'
        'aufs5-loopback.patch'
        'aufs5-mmap.patch'
        'aufs5-standalone.patch'
        'tmpfs-idr.patch'
        'vfs-ino.patch'
        # ARCH Patches
        '0001-ZEN-Add-sysctl-and-CONFIG-to-disallow-unprivileged-CLONE_NEWUSER.patch'
        # MANJARO Patches
        #"prepatch-${_basekernel}.patch"
        '0001-nonupstream-navi10-vfio-reset.patch'
        '0001-i2c-nuvoton-nc677x-hwmon-driver.patch'
        '0001-apparmor-patch-to-provide-compatibility-with-v2-net-rules.patch'
        '0002-apparmor-af_unix-mediation.patch'
        '0003-apparmor-fix-use-after-free-in-sk_peer_label.patch'
        '0004-apparmor-fix-apparmor-mediating-locking-non-fs-unix-sockets.patch'
        # Lenovo P50 multiple fans
        '0005-thinkpad_acpi_dual_fan_control.patch::https://github.com/dvhart/linux-pdx86/commit/26c16f9d956f269bbc32e034e3ec11c4831137de.patch'
        # Oracle
        '0001-linux-dmjordan.git-5caab6aa6a673469e451ecdd018c5a42b2fb1f10.patch'
        '0002-linux-dmjordan.git-018908fd0f9a56156bc34bc86781a7877c3d4d20.patch'
        '0003-linux-dmjordan.git-14beeebb8bff7b5f1baed7648a0e050d7a74012e.patch'
        '0004-linux-dmjordan.git-62075c45f01af2c4c1fc6f315bd7cfc9c3a3c1ee.patch'
        '0005-linux-dmjordan.git-5d7bb66ae309681715b44acdc8d17c450592e77a.patch'
        '0006-linux-dmjordan.git-e26200a16b12befc4f2be816ef1f6f0a0b34653d.patch'
        '0007-linux-dmjordan.git-0e955dc47a08815500de2f559d0e6781622cbbf2.patch'
        '0008-linux-dmjordan.git-09828a28b104334ea5d1744fdfb525bfc51549b3.patch'
        '0009-linux-dmjordan.git-b87c24b69608305c65161165eb07460ecddb8a70.patch'
        '0010-linux-dmjordan.git-dacbf15ae1e2027e71eb1ef45ea4d831189923dc.patch'
        # Bootsplash
        '0001-bootsplash.patch'
        '0002-bootsplash.patch'
        '0003-bootsplash.patch'
        '0004-bootsplash.patch'
        '0005-bootsplash.patch'
        '0006-bootsplash.patch'
        '0007-bootsplash.patch'
        '0008-bootsplash.patch'
        '0009-bootsplash.patch'
        '0010-bootsplash.patch'
        '0011-bootsplash.patch'
        '0012-bootsplash.patch'
        '0013-bootsplash.patch'
        #mbp
        '2001-drm-amd-display-Force-link_rate-as-LINK_RATE_RBR2-fo.patch'
        '3001-applesmc-convert-static-structures-to-drvdata.patch'
        '3002-applesmc-make-io-port-base-addr-dynamic.patch'
        '3003-applesmc-switch-to-acpi_device-from-platform.patch'
        '3004-applesmc-key-interface-wrappers.patch'
        '3005-applesmc-basic-mmio-interface-implementation.patch'
        '3006-applesmc-fan-support-on-T2-Macs.patch'
        '4001-touchpad.patch'
        '4002-keyboard-backlight.patch'
        '5001-brcmfmac-move-brcmf_mp_device-into-its-own-header.patch'
        '5002-brcmfmac-Add-ability-to-manually-specify-FW-rambase-.patch'
        'camera.patch'
        'sphinx-workaround.patch'
        'wifi.patch')
sha256sums=('e342b04a2aa63808ea0ef1baab28fc520bd031ef8cf93d9ee4a31d4058fcb622'
            '523e014b8432252f9739216e63811e60e6f8da5318122ec880c24d752a493e0f'
            'a99cf4d0134819e17a068085dcebb7b87225403e01b336c6fb7739aac80aff5b'
            '659042e36197e169ca91c751be1d463478e62d315c0ae8514c619426409316be'
            'b44d81446d8b53d5637287c30ae3eb64cae0078c3fbc45fcf1081dd6699818b5'
            '0692136bde829e8eabb810d9e7cd553558756e89ddf13161a0604b44e87a230d'
            '31e2f0ed876e605a300ec14e6b5574163b3400f069df13f43faad24f0c91a696'
            '5f420b7578c402448a94d37ec156b22cd3cc009a418423629b699855c5f97156'
            '998ff0d18c67521380e6bc0cf363baaf93129a4ac3d24320491e6c00d84a17a1'
            '69d56e5d191e4e6cbca31bf0197af208d21fad6256ae61bcef769fa57a0c8960'
            '22b5e9517a15906c8eccebe09393efd91db67aa7ebf9ec8e653e87dd07963137'
            '9203ec78b9f6000f9f3d094316f355eeab9488847192dca0d6346d159bb17097'
            '20abad2643c635210c925c3ce3a12eb31f813819d6e661c6d99d9cc3163fbef7'
            '7685d526bbdbfa795986591a70071c960ff572f56d3501774861728a9df8664c'
            'f1eec160ce5df5c2ea58d4e4fd44a6b1013863c6b3bf649414cd18c89ae500fa'
            '0556859a8168c8f7da9af8e2059d33216d9e5378d2cac70ca54c5ff843fa5add'
            '98202b8ad70d02d86603294bae967874fa7b18704b5c7b867568b0fd33a08921'
            '5cbbf3db9ea3205e9b89fe3049bea6dd626181db0cb0dc461e4cf5a400c68dd6'
            'c7dbec875d0c1d6782c037a1dcefff2e5bdb5fc9dffac1beea07dd8c1bdef1d7'
            '77746aea71ffb06c685e7769b49c78e29af9b2e28209cd245e95d9cbb0dba3c9'
            'f93707e75ec6be5f289605f913e59d4f3514524a1aab3368f49bf6789723d443'
            'b1a652de71740444bc111056921d4cdce9cca03c54d1ef1533355482621b3097'
            'bd54f08a4bb4ef63585c3a995e7554635dd275aa22f08dc8fea5ca4267736771'
            'c0f407f3860609326a7415c9bbda2c5e39a0a97ea9e831d0ab82f2f7a3480614'
            'b8dfcc90b0233947b4d44bf8dd207024df7f02b80faaab4111e4c49a198cc725'
            '6d778ef836f4e65b5822f501d70acdae63f20ba6934d070f360cbe0e4575e6c2'
            '5b379366b7e122052cf9ae8e794c8049e92313b060f0493a669602e9e15d46e4'
            '6e3974c6e4e2702097ed2538acc4b8cd1577445738e41368b12191e016ab4489'
            '3fd57bbf4a5b17b3d058f667e9b34b9ed378523985abb15f6d394ae50b2fcc3d'
            '740c9bb706cb7abcbde245df782b945bbe5cdda017d4b94b6044b1db487858e2'
            'eb927a0d698b49632ad0f85b84a18173866d51719c9d2057080189b7747f5fcb'
            'a504f6cf84094e08eaa3cc5b28440261797bf4f06f04993ee46a20628ff2b53c'
            'e096b127a5208f56d368d2cb938933454d7200d70c86b763aa22c38e0ddb8717'
            '8c1c880f2caa9c7ae43281a35410203887ea8eae750fe8d360d0c8bf80fcc6e0'
            '1144d51e5eb980fceeec16004f3645ed04a60fac9e0c7cf88a15c5c1e7a4b89e'
            'dd4b69def2efacf4a6c442202ad5cb93d492c03886d7c61de87696e5a83e2846'
            '028b07f0c954f70ca37237b62e04103e81f7c658bb8bd65d7d3c2ace301297dc'
            'c8b0cb231659d33c3cfaed4b1f8d7c8305ab170bdd4c77fce85270d7b6a68000'
            '8dbb5ab3cb99e48d97d4e2f2e3df5d0de66f3721b4f7fd94a708089f53245c77'
            'a7aefeacf22c600fafd9e040a985a913643095db7272c296b77a0a651c6a140a'
            'e9f22cbb542591087d2d66dc6dc912b1434330ba3cd13d2df741d869a2c31e89'
            '27471eee564ca3149dd271b0817719b5565a9594dc4d884fe3dc51a5f03832bc'
            '60e295601e4fb33d9bf65f198c54c7eb07c0d1e91e2ad1e0dd6cd6e142cb266d'
            '035ea4b2a7621054f4560471f45336b981538a40172d8f17285910d4e0e0b3ef'
            '8e8fb392a95f71ae63df14199b9671a75a7e819e75d54a6e2767d6ea5b86bc6a'
            '25e1aac0d44d72e377f08e4f4b90351cffcacc0be63e02a4033cb99f10cc9fe7'
            'c70118659c5cf6a5c7f060c941d46fdd3b1e6d28f2b62c24a941745f2b3c4732'
            '3855aa07fab97d202900216951225b6952d7c716258a3c3727df8e6277289ee0'
            '9e5e0b45fe007ed214049b26b44174ee8f61376076e80fd33bba9fdac001e157'
            '3c8a361370ed3ee094e2c8af1ff5360fd78f24e387c250904031fb70e8f2bb6e'
            '8e43d95104301913737e5d73860f0e21bb0e5e25dcfd0f16d48a0715b38c98a1'
            'e1d72fdb0a7a66a6f3fc8afb6fe056f28cfa088c1cc9c799b93405b62a274b96'
            'a6c070d7b7444d711d9cb6b28bccb774228864132ef83dd3a291df3353e85465'
            '0318952f59efdce4dc72703adc764940db6fdff184960c27a23a80c3413d8a60'
            'e632f2959efca848fd28acb5e278cc476f8fb54d70ca95272b0a76add47e474e'
            '717f7fc70a3e3fcfa5ffbac505c8259c1d86718ca1ca6593e8925dac3d29a835'
            '8cb21e0b3411327b627a9dd15b8eb773295a0d2782b1a41b2a8839d1b2f5778c'
            '2a496b5e976e8371e5c1fa8e2102c19481fa72bcdc97df7fe224a1aef8c32609')

prepare() {
  cd "${srcdir}/linux-${_basekernel}"

  msg "add upstream patch"
  patch -p1 -i "${srcdir}/patch-${pkgver}"

  # add latest fixes from stable queue, if needed
  # http://git.kernel.org/?p=linux/kernel/git/stable/stable-queue.git
  # enable only if you have "gen-stable-queue-patch.sh" executed before
  #patch -Np1 -i "${srcdir}/prepatch-${_basekernel}.patch"

  msg "disable USER_NS for non-root users"
  patch -Np1 -i "${srcdir}/0001-ZEN-Add-sysctl-and-CONFIG-to-disallow-unprivileged-CLONE_NEWUSER.patch"

  msg "oracle patches"
  msg2 "0001-linux-dmjordan"
  patch -Np1 -i "${srcdir}/0001-linux-dmjordan.git-5caab6aa6a673469e451ecdd018c5a42b2fb1f10.patch"
  msg2 "0002-linux-dmjordan"
  patch -Np1 -i "${srcdir}/0002-linux-dmjordan.git-018908fd0f9a56156bc34bc86781a7877c3d4d20.patch"
  msg2 "0003-linux-dmjordan"
  patch -Np1 -i "${srcdir}/0003-linux-dmjordan.git-14beeebb8bff7b5f1baed7648a0e050d7a74012e.patch"
  msg2 "0004-linux-dmjordan"
  patch -Np1 -i "${srcdir}/0004-linux-dmjordan.git-62075c45f01af2c4c1fc6f315bd7cfc9c3a3c1ee.patch"
  msg2 "0005-linux-dmjordan"
  patch -Np1 -i "${srcdir}/0005-linux-dmjordan.git-5d7bb66ae309681715b44acdc8d17c450592e77a.patch"
  msg2 "0006-linux-dmjordan"
  patch -Np1 -i "${srcdir}/0006-linux-dmjordan.git-e26200a16b12befc4f2be816ef1f6f0a0b34653d.patch"
  msg2 "0007-linux-dmjordan"
  patch -Np1 -i "${srcdir}/0007-linux-dmjordan.git-0e955dc47a08815500de2f559d0e6781622cbbf2.patch"
  msg2 "0008-linux-dmjordan"
  patch -Np1 -i "${srcdir}/0008-linux-dmjordan.git-09828a28b104334ea5d1744fdfb525bfc51549b3.patch"
  msg2 "0009-linux-dmjordan"
  patch -Np1 -i "${srcdir}/0009-linux-dmjordan.git-b87c24b69608305c65161165eb07460ecddb8a70.patch"
  msg2 "0010-linux-dmjordan"
  patch -Np1 -i "${srcdir}/0010-linux-dmjordan.git-dacbf15ae1e2027e71eb1ef45ea4d831189923dc.patch"
  
  msg "snapd patches"
  # https://gitlab.com/apparmor/apparmor-kernel/tree/5.2-outoftree
  msg2 "0001-apparmor-patch-to-provide-compatibility-with-v2-net-rules"
  patch -Np1 -i "${srcdir}/0001-apparmor-patch-to-provide-compatibility-with-v2-net-rules.patch"
  msg2 "0002-apparmor-af_unix-mediation"
  patch -Np1 -i "${srcdir}/0002-apparmor-af_unix-mediation.patch"
  msg2 "0003-apparmor-fix-use-after-free-in-sk_peer_label"
  patch -Np1 -i "${srcdir}/0003-apparmor-fix-use-after-free-in-sk_peer_label.patch"
  msg2 "0004-apparmor-fix-apparmor-mediating-locking-non-fs-unix-sockets"
  patch -Np1 -i "${srcdir}/0004-apparmor-fix-apparmor-mediating-locking-non-fs-unix-sockets.patch"

  msg "navi10-vfio reset patch"
  # TODO: remove when AMD properly fixes it!
  # INFO: this is a hack and won't be upstreamed
  # https://forum.level1techs.com/t/145666/86
  # https://forum.manjaro.org/t/107820/11
  patch -Np1 -i "${srcdir}/0001-nonupstream-navi10-vfio-reset.patch"

  msg "nuvoton hwmon driver patch"
  # https://twitter.com/vskye11/status/1216240051639791616
  patch -Np1 -i '../0001-i2c-nuvoton-nc677x-hwmon-driver.patch'
  
  msg "multiple fans on Lenovo P50"
  # https://github.com/vmatare/thinkfan/issues/58
  patch -Np1 -i "${srcdir}/0005-thinkpad_acpi_dual_fan_control.patch"

  msg "bootsplash patches"
  # http://lkml.iu.edu/hypermail/linux/kernel/1710.3/01542.html
  msg2 "0001-bootsplash."
  patch -Np1 -i "${srcdir}/0001-bootsplash.patch"
  msg2 "0002-bootsplash."
  patch -Np1 -i "${srcdir}/0002-bootsplash.patch"
  msg2 "0003-bootsplash."
  patch -Np1 -i "${srcdir}/0003-bootsplash.patch"
  msg2 "0004-bootsplash."
  patch -Np1 -i "${srcdir}/0004-bootsplash.patch"
  msg2 "0005-bootsplash."
  patch -Np1 -i "${srcdir}/0005-bootsplash.patch"
  msg2 "0006-bootsplash."
  patch -Np1 -i "${srcdir}/0006-bootsplash.patch"
  msg2 "0007-bootsplash."
  patch -Np1 -i "${srcdir}/0007-bootsplash.patch"
  msg2 "0008-bootsplash."
  patch -Np1 -i "${srcdir}/0008-bootsplash.patch"
  msg2 "0009-bootsplash."
  patch -Np1 -i "${srcdir}/0009-bootsplash.patch"
  msg2 "0010-bootsplash."
  patch -Np1 -i "${srcdir}/0010-bootsplash.patch"
  msg2 "0011-bootsplash."
  patch -Np1 -i "${srcdir}/0011-bootsplash.patch"
  msg2 "0012-bootsplash."
  patch -Np1 -i "${srcdir}/0012-bootsplash.patch"
  # use git-apply to add binary files
  msg2 "0013-bootsplash."
  git apply -p1 < "${srcdir}/0013-bootsplash.patch"

  msg "add aufs5 support"
  msg2 "aufs5.6-${_aufs}"
  patch -Np1 -i "${srcdir}/aufs5.6-${_aufs}.patch"
  msg2 "aufs5-base"
  patch -Np1 -i "${srcdir}/aufs5-base.patch"
  msg2 "aufs5-kbuild"
  patch -Np1 -i "${srcdir}/aufs5-kbuild.patch"
  msg2 "aufs5-loopback"
  patch -Np1 -i "${srcdir}/aufs5-loopback.patch"
  msg2 "aufs5-mmap"
  patch -Np1 -i "${srcdir}/aufs5-mmap.patch"
  msg2 "aufs5-standalone"
  patch -Np1 -i "${srcdir}/aufs5-standalone.patch"
  msg2 "tmpfs-idr"
  patch -Np1 -i "${srcdir}/tmpfs-idr.patch"
  msg2 "vfs-ino"
  patch -Np1 -i "${srcdir}/vfs-ino.patch"

    #add mbp support
  msg "add mbp support"
  msg2 "drm-amd-display-force-link-rate"
  patch -Np1 -i "${srcdir}/2001-drm-amd-display-Force-link_rate-as-LINK_RATE_RBR2-fo.patch"
  msg2 "applesmc-convert-static-structures-to-drvdata"
  patch -Np1 -i "${srcdir}/3001-applesmc-convert-static-structures-to-drvdata.patch"
  msg2 "applesmc-switch-to-acpi-device-from-platform"
  patch -Np1 -i "${srcdir}/3002-applesmc-make-io-port-base-addr-dynamic.patch"
  msg2 "applesmc-switch-to-acpi_device-from-platform"
  patch -Np1 -i "${srcdir}/3003-applesmc-switch-to-acpi_device-from-platform.patch"
  msg2 "applesmc-key-interface-wrappers"
  patch -Np1 -i "${srcdir}/3004-applesmc-key-interface-wrappers.patch"
  msg2 "applesmc-basic-mmio-interface-implementation"
  patch -Np1 -i "${srcdir}/3005-applesmc-basic-mmio-interface-implementation.patch"
  msg2 "applesmc-fan-support-on-T2-Macs"
  patch -Np1 -i "${srcdir}/3006-applesmc-fan-support-on-T2-Macs.patch"
  msg2 "touchpad"
  patch -Np1 -i "${srcdir}/4001-touchpad.patch"
  msg2 "keyboard-backlight"
  patch -Np1 -i "${srcdir}/4002-keyboard-backlight.patch"
  msg2 "brcmfmac-move-brcmf_mp_device-into-its-own-header"
  patch -Np1 -i "${srcdir}/5001-brcmfmac-move-brcmf_mp_device-into-its-own-header.patch"
  msg2 "brcmfmac-Add-ability-to-manually-specify-FW-rambase"
  patch -Np1 -i "${srcdir}/5002-brcmfmac-Add-ability-to-manually-specify-FW-rambase-.patch"
  msg2 "camera"
  patch -Np1 -i "${srcdir}/camera.patch"
  msg2 "sphinx-workaround"
  patch -Np1 -i "${srcdir}/sphinx-workaround.patch"
  msg2 "wifi"
  patch -Np1 -i "${srcdir}/wifi.patch"

  if [ "${CARCH}" = "x86_64" ]; then
    cat "${srcdir}/config.x86_64" > ./.config
  else
    cat "${srcdir}/config" > ./.config
  fi

  cat "${srcdir}/config.aufs" >> ./.config

  if [ "${_kernelname}" != "" ]; then
    sed -i "s|CONFIG_LOCALVERSION=.*|CONFIG_LOCALVERSION=\"${_kernelname}\"|g" ./.config
    sed -i "s|CONFIG_LOCALVERSION_AUTO=.*|CONFIG_LOCALVERSION_AUTO=n|" ./.config
  fi

  msg "set extraversion to pkgrel"
  sed -ri "s|^(EXTRAVERSION =).*|\1 -${pkgrel}|" Makefile

  msg "don't run depmod on 'make install'"
  # We'll do this ourselves in packaging
  sed -i '2iexit 0' scripts/depmod.sh

  msg "get kernel version"
  make prepare

  # load configuration
  # Configure the kernel. Replace the line below with one of your choice.
  #make menuconfig # CLI menu for configuration
  #make nconfig # new CLI menu for configuration
  #make xconfig # X-based configuration
  #make oldconfig # using old config from previous kernel version
  # ... or manually edit .config

  msg "rewrite configuration"
  yes "" | make config >/dev/null
}

build() {
  cd "${srcdir}/linux-${_basekernel}"

  msg "build"
  make ${MAKEFLAGS} LOCALVERSION= bzImage modules
}

package_linux56-mbp() {
  pkgdesc="The ${pkgbase/linux/Linux} kernel and modules"
  depends=('coreutils' 'linux-firmware' 'kmod' 'mkinitcpio>=27')
  optdepends=('crda: to set the correct wireless channels of your country')
  provides=("linux=${pkgver}" VIRTUALBOX-GUEST-MODULES WIREGUARD-MODULE)
  install=linux56.install

  cd "${srcdir}/linux-${_basekernel}"

  KARCH=x86

  # get kernel version
  _kernver="$(make LOCALVERSION= kernelrelease)"

  mkdir -p "${pkgdir}"/{boot,usr/lib/modules}
  make LOCALVERSION= INSTALL_MOD_PATH="${pkgdir}/usr" modules_install

  # systemd expects to find the kernel here to allow hibernation
  # https://github.com/systemd/systemd/commit/edda44605f06a41fb86b7ab8128dcf99161d2344
  cp arch/$KARCH/boot/bzImage "${pkgdir}/usr/lib/modules/${_kernver}/vmlinuz"

  # Used by mkinitcpio to name the kernel
  echo "${pkgbase}" | install -Dm644 /dev/stdin "${pkgdir}/usr/lib/modules/${_kernver}/pkgbase"
  echo "${_basekernel}-${CARCH}-mbp" | install -Dm644 /dev/stdin "${pkgdir}/usr/lib/modules/${_kernver}/kernelbase"

  # add kernel version
  if [ "${CARCH}" = "x86_64" ]; then
     echo "${pkgver}-${pkgrel}-MANJARO-mbp x64" > "${pkgdir}/boot/${pkgbase}-${CARCH}.kver"
  else
     echo "${pkgver}-${pkgrel}-MANJARO-mbp x32" > "${pkgdir}/boot/${pkgbase}-${CARCH}.kver"
  fi

  # make room for external modules
  local _extramodules="extramodules-${_basekernel}${_kernelname:--MANJARO-mbp}"
  ln -s "../${_extramodules}" "${pkgdir}/usr/lib/modules/${_kernver}/extramodules"

  # add real version for building modules and running depmod from hook
  echo "${_kernver}" |
    install -Dm644 /dev/stdin "${pkgdir}/usr/lib/modules/${_extramodules}/version"

  # remove build and source links
  rm "${pkgdir}"/usr/lib/modules/${_kernver}/{source,build}

  # now we call depmod...
  depmod -b "${pkgdir}/usr" -F System.map "${_kernver}"

  # add vmlinux
  install -Dt "${pkgdir}/usr/lib/modules/${_kernver}/build" -m644 vmlinux
}

package_linux56-mbp-headers() {
  pkgdesc="Header files and scripts for building modules for ${pkgbase/linux/Linux} kernel"
  provides=("linux-headers=$pkgver")

  cd "${srcdir}/linux-${_basekernel}"
  local _builddir="${pkgdir}/usr/lib/modules/${_kernver}/build"

  install -Dt "${_builddir}" -m644 Makefile .config Module.symvers
  install -Dt "${_builddir}/kernel" -m644 kernel/Makefile

  mkdir "${_builddir}/.tmp_versions"

  cp -t "${_builddir}" -a include scripts

  install -Dt "${_builddir}/arch/${KARCH}" -m644 "arch/${KARCH}/Makefile"
  install -Dt "${_builddir}/arch/${KARCH}/kernel" -m644 "arch/${KARCH}/kernel/asm-offsets.s"
  #install -Dt "${_builddir}/arch/${KARCH}/kernel" -m644 "arch/${KARCH}/kernel/macros.s"

  if [ "${CARCH}" = "i686" ]; then
    install -Dt "${_builddir}/arch/${KARCH}" -m644 "arch/${KARCH}/Makefile_32.cpu"
  fi

  cp -t "${_builddir}/arch/${KARCH}" -a "arch/${KARCH}/include"

  install -Dt "${_builddir}/drivers/md" -m644 drivers/md/*.h
  install -Dt "${_builddir}/net/mac80211" -m644 net/mac80211/*.h

  # http://bugs.archlinux.org/task/13146
  install -Dt "${_builddir}/drivers/media/i2c" -m644 drivers/media/i2c/msp3400-driver.h

  # http://bugs.archlinux.org/task/20402
  install -Dt "${_builddir}/drivers/media/usb/dvb-usb" -m644 drivers/media/usb/dvb-usb/*.h
  install -Dt "${_builddir}/drivers/media/dvb-frontends" -m644 drivers/media/dvb-frontends/*.h
  install -Dt "${_builddir}/drivers/media/tuners" -m644 drivers/media/tuners/*.h

  # add xfs and shmem for aufs building
  mkdir -p "${_builddir}"/{fs/xfs,mm}

  # copy in Kconfig files
  find . -name Kconfig\* -exec install -Dm644 {} "${_builddir}/{}" \;

  if [ "${CARCH}" = "x86_64" ]; then
    # add objtool for external module building and enabled VALIDATION_STACK option
    install -Dt "${_builddir}/tools/objtool" tools/objtool/objtool
  fi

  # remove unneeded architectures
  local _arch
  for _arch in "${_builddir}"/arch/*/; do
    [[ ${_arch} == */x86/ ]] && continue
    rm -r "${_arch}"
  done

  # remove files already in linux-docs package
  # rm -r "${_builddir}/Documentation"

  # Fix permissions
  chmod -R u=rwX,go=rX "${_builddir}"

  # strip scripts directory
  local _binary _strip
  while read -rd '' _binary; do
    case "$(file -bi "${_binary}")" in
      *application/x-sharedlib*)  _strip="${STRIP_SHARED}"   ;; # Libraries (.so)
      *application/x-archive*)    _strip="${STRIP_STATIC}"   ;; # Libraries (.a)
      *application/x-executable*) _strip="${STRIP_BINARIES}" ;; # Binaries
      *) continue ;;
    esac
    /usr/bin/strip ${_strip} "${_binary}"
  done < <(find "${_builddir}/scripts" -type f -perm -u+w -print0 2>/dev/null)
}

package_linux56-mbp-docs() {
  pkgdesc="Documentation for the $pkgdesc kernel"

  cd "${srcdir}/linux-${_basekernel}"
  local builddir="$pkgdir/usr/lib/modules/$(<version)/build"

  echo "Installing documentation..."
  local src dst
  while read -rd '' src; do
    dst="${src#Documentation/}"
    dst="$builddir/Documentation/${dst#output/}"
    install -Dm644 "$src" "$dst"
  done < <(find Documentation -name '.*' -prune -o ! -type d -print0)

  echo "Adding symlink..."
  mkdir -p "$pkgdir/usr/share/doc"
  ln -sr "$builddir/Documentation" "$pkgdir/usr/share/doc/$pkgbase"
}

_server=cpx51

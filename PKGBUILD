# Maintainer: Fansure Grin <quarlong@qq.com>
pkgname=trojan-qt5
_foldname=Trojan-Qt5
pkgver=1.4.0
pkgrel=1
pkgdesc="A cross-platform Socks5/Http/SS/SSR/Vmess/Trojan(go)/Snell GUI client"
arch=("x86_64")
license=("GPL")
url="https://github.com/fansuregrin/trojan-qt5-bak"
source=("https://github.com/fansuregrin/trojan-qt5-bak/releases/download/V1.4.0/Trojan-Qt5.tar.xz")
sha512sums=("e5aa347d6997565c4b21899271816a6aa6a76cea18502b18aebf80392a9d3d48c87a60902b33623ca738b626d432049920d87a44468ff01a734b0f2beea75072")
options=(!strip)
package(){
	install -Dvdm755 "${pkgdir}/opt/${pkgname}/usr"		
	install -Dvdm755 "${pkgdir}/usr/bin"
	install -Dvdm755 "${pkgdir}/usr/share"	
	cp -r "${_foldname}/usr/bin" "${_foldname}/usr/lib" "${_foldname}/usr/plugins" "${_foldname}/usr/translations" "${pkgdir}/opt/${pkgname}/usr"
	cp -r "${_foldname}/usr/share/applications" "${_foldname}/usr/share/doc" "${_foldname}/usr/share/icons" "${_foldname}/usr/share/licenses" "${pkgdir}/usr/share"
	ln -sf "/opt/${pkgname}/usr/bin/${pkgname}" "${pkgdir}/usr/bin/${pkgname}"
}

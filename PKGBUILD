# Maintainer: Artoria Pendragon <saber-nyan@ya.ru>
# Hooks: https://www.reddit.com/r/archlinux/comments/4zrsc3/keep_your_system_fully_functional_after_a_kernel/d6yin0r/
pkgname=kernel-modules-hook
pkgver=0.1.7
pkgrel=1
pkgdesc="Keeps your system fully functional after a kernel upgrade"
arch=('any')
url="https://github.com/sparques/kernel-modules-hook"
license=('UNLICENSE')
install="${pkgname}.install"
source=(
	"10-linux-modules-pre.hook"
	"10-linux-modules-post.hook"
		"UNLICENSE")

package() {
	install -Dm644 '10-linux-modules-pre.hook' "${pkgdir}/usr/share/libalpm/hooks/10-linux-modules-pre.hook"
	install -Dm644 '10-linux-modules-post.hook' "${pkgdir}/usr/share/libalpm/hooks/10-linux-modules-post.hook"
	install -Dm644 'UNLICENSE' "${pkgdir}/usr/share/licenses/${pkgname}/UNLICENSE"
}

sha256sums=('b0e294715725f7e6d7fb9b2332364bd3a8c4f8cbc931f7f4668e057dd60c2a29'
            'dfb3e7f681d75145ca2bc1ec0d78b6a3a07b690285676a411687a8b7073d63bf'
            '7e12e5df4bae12cb21581ba157ced20e1986a0508dd10d0e8a4ab9a4cf94e85c')

# Generated by gem2arch (https://github.com/anatol/gem2arch)
# Maintainer: kusakata <shohei atmark kusakata period com>

_gemname=shoulda-context
pkgname=ruby-$_gemname
pkgver=1.1.6
pkgrel=1
pkgdesc='Context framework extracted from Shoulda'
arch=(any)
url='http://thoughtbot.com/community/'
license=(MIT)
depends=(ruby)
options=(!emptydirs)
source=(https://rubygems.org/downloads/$_gemname-$pkgver.gem)
noextract=($_gemname-$pkgver.gem)
sha1sums=('ede236a3bf1d9dc8c5e279c59131ac019f8210b8')

package() {
  local _gemdir="$(ruby -e'puts Gem.default_dir')"
  gem install --ignore-dependencies --no-user-install -i "$pkgdir/$_gemdir" -n "$pkgdir/usr/bin" $_gemname-$pkgver.gem
  rm "$pkgdir/$_gemdir/cache/$_gemname-$pkgver.gem"
  install -D -m644 "$pkgdir/$_gemdir/gems/$_gemname-$pkgver/MIT-LICENSE" "$pkgdir/usr/share/licenses/$pkgname/MIT-LICENSE"
}

# This PKGBUILD was generated by cpan4pacman via CPANPLUS::Dist::Pacman
# Contributor: François Charette <firmicus ατ gmx δοτ net>

pkgname=perl-paranoid
pkgver=0.20
pkgrel=1
pkgdesc="Paranoia support for safer programs"
arch=('i686' 'x86_64')
url="http://search.cpan.org/~Paranoid/Paranoid"
license=('GPL' 'PerlArtistic')
depends=('perl')
options=('!emptydirs')
source=(http://www.cpan.org/authors/id/C/CO/CORLISS/Paranoid/Paranoid-$pkgver.tar.gz) 
md5sums=('f3a0d48d15eeb45d18b57c7898172c01')

build() {
  cd  $startdir/src/Paranoid-$pkgver
  PERL_MM_USE_DEFAULT=1 perl Makefile.PL INSTALLDIRS=vendor || return 1 
  make || return 1
  make install DESTDIR=$startdir/pkg || return 1
  find $startdir/pkg -name '.packlist' -delete
  find $startdir/pkg -name '*.pod' -delete
}

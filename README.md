
# Hugo Academic

## Setup

Install hugo:

```bash
cd $HOME
mkdir $HOME/bin/
wget https://github.com/gohugoio/hugo/releases/download/v0.80.0/hugo_extended_0.80.0_macOS-64bit.tar.gz
tar -zxvf hugo_extended_0.80.0_macOS-64bit.tar.gz -C bin/
rm -f hugo_extended_0.80.0_macOS-64bit.tar.gz bin/README bin/LICENSE
```

Make sure that `$HOME/bin/` is in your `$PATH`.

Clone repository:

```bash
git clone git@github.com:EmelineBolmont/hugo-academic.git
cd hugo-academic/
git submodule update --init --recursive
```

## Run on your local machine

Start local hugo server:

```bash
cd hugo-academic/
hugo server -D
```

Visit your site on your local machine via [http://localhost:1313](http://localhost:1313). Any modification will automatically appear in the website running on your local machine.

## Key files

- `content/en/authors/admin/_index.md`: Biography
- `content/en/home/science.md`: Science
- `content/en/project/posidonius/index.md`: Project Posidonius
- `content/en/project/mercury-t/index.md`: Project Mercury-T

The French version files have the same path but `fr` instead of `en`.

## Source

Based on [academic-kickstart](https://github.com/sourcethemes/academic-kickstart/) by [George Cushen](https://georgecushen.com).


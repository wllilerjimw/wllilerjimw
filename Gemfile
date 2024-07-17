# frozen_string_literal: true

source "https://rubygems.org"

gem "jekyll-theme-chirpy", "~> 6.0", ">= 6.0.1"

# 针对 Windows 和 JRuby，包含时区相关的 gem
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

# 提高在 Windows 上监视目录的性能
gem "wdm", "~> 0.1.1", platforms: [:mingw, :x64_mingw, :mswin]

# 针对 JRuby，锁定 http_parser.rb 版本
gem "http_parser.rb", "~> 0.6.0", platforms: [:jruby]

# 针对 Linux-musl，锁定 jekyll-sass-converter 版本
if RUBY_PLATFORM =~ /linux-musl/
  gem "jekyll-sass-converter", "~> 2.0"
end

# 添加 HTML-Proofer 用于检查 HTML 文件
gem "html-proofer"
= csvscan

https://github.com/n6udp/csvscan

== DESCRIPTION:

Updated for Ruby 2.X

This is a packaged version of CSVScan, written by MoonWolf. If you can read Japanese, checkout README.old.ja for whatever he said.

On a 10,000 line file:

    time cat example.csv | ruby fastercsv_benchmark.rb

    real	0m8.804s
    user	0m8.502s
    sys	0m0.304s

    time cat example.csv | ruby csvscan_benchmark.rb 

    real	0m0.860s
    user	0m0.782s
    sys	0m0.088s


== FEATURES/PROBLEMS:

* Ruby 2.X support

== SYNOPSIS:

    require 'csvscan'
    CSVScan.scan(STDIN) do |row|
        puts row.inspect
    end

== REQUIREMENTS:

* c compiler
* ruby 2.X

== INSTALL:

* gem install n6udp-csvscan --source http://gems.github.com

== LICENSE:

LGPL (original license)

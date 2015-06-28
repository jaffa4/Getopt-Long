Getopt-Long
========



Getopt::Long

It is based on Getopt::Long (2.47) Perl 5 module. See Getopt::Long Perl 5 documentation.
It is in Alpha state.

Usage:

use Getopt::Long;
my $data   = "file.dat";
my $length = 24;
my $verbose;
say "before";
GetOptions ("length=i" => \$length,    # numeric
              "file=s"   => \$data,      # string
              "verbose"  => \$verbose)   # flag
  or die("Error in command line arguments\n");

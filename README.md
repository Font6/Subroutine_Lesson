# Subroutine_Lesson

#!/usr/bin/env perl
use strict;
use warnings;

my %Man = (
    mfirst     => 'Jon',
    mlast      => 'Smith',
    mincome    => '70000',
);

my %Woman = (
    wfirst     => 'Jane',
    wlast      => 'Doe',
    wincome    => '50000',
);

my $Family_Income = add($Man{mincome}, $Woman{wincome});
my $HusbandName = "$Man{mfirst} $Man{mlast}";
my $WifeName = "$Woman{wfirst} $Man{mlast}";;

print "$Family_Income, $HusbandName, $WifeName\n";

sub add {
    
    return $Man{mincome} + $Woman{wincome};
}

1;

Title: Minor changes in the fields of Campaigns 11, 12, and 13
Date: 2016-01-28 16:00
Author: Geert Barentsen

K2 users are alerted to a small but necessary adjustment
in the position of Campaigns 11, 12, and 13,
for which target proposals are currently being solicited as part of the
[K2 Guest Observer Cycle 4](call-for-k2-go-cycle-4-proposals-for-campaigns-11-12-and-13.html).

The change, explained below, alters ~0.2% of sky area covered
and is unlikely to affect the vast majority of proposals.
All users are nevertheless encouraged to update the
<a href="software.html#k2fov">K2fov</a> target selection tool
to version 4.0, which was released on 27 Jan 2016 to include the change.

K2fov can be updated from the command line using pip:

    pip install K2fov --upgrade

The version number of your K2fov installation may be verified
using the following command:

    python -c "import pkg_resources; print(pkg_resources.require('K2fov')[0].version)"

This should return "4.0.0" or higher.


### Background

Campaigns 11, 12, and 13 are being rotated slightly to
accommodate a change in the configuration of the Kepler spacecraft.

During these Campaigns, spacecraft telemetry will be downlinked
using a different low-gain antenna than before:
<i>LGA2</i> instead of <i>LGA1</i>.
This antenna provides a better orientation to Earth
and compensates for the increasing range
of the spacecraft to the Earth (now 0.8 AU).

The change of antenna was recently trialled during Campaign 7,
where it was found to cause a small increase in the roll drift rate.
The reduced pointing performance was understood to be caused
by the antenna's radiation pressure,
which torques the spacecraft slightly differently when <i>LGA2</i> is used,
increasing the roll rate.

To optimize fuel usage and photometric precision,
the K2 team has decided to adjust the roll angle
of Campaigns 11, 12, and 13 by a very small amount
(0.12--0.16 degrees) to optimally balance the spacecraft
against solar pressure and antenna radiation
when <i>LGA2</i> is in use.

As a consequence, there is a minor change in the fields of view covered by K2
during these campaigns. The position of the CCD edges
are being shifted by ~0.5 arcsec (~0.1 px) near the center of the
focal plane, and by up to 60 arcsec (~15 px) near the corners.
The change is illustrated in the figure below,
which shows the change in sky coverage for a single CCD channel
near the corner of C11,
where the shift is the most significant.

Please [contact the Guest Observer Office](helpdesk.html) if you have questions.

<div class="thumbnail col-sm-6">
<a href="images/news/c11-roll-change-in-channel-71.png"><img src="images/news/c11-roll-change-in-channel-71.png" alt="C11 Roll Change" class="img-responsive" style="max-width:500px;"></a>
<div class="caption">
<i>Figure: Illustration of the effect of the change in sky coverage
for one of the CCD detectors near the corner of the focal plane during K2 Campaign 11.  The edges of the field are shifted by up to ~60 arcsec.</i>
</div>
</div>

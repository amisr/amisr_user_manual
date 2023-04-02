# SRI Data Format

AMISR data is available in the SRI data format from the SRI AMISR website.  The files in the Madrigal database contain most of the same fields, but the array structuring in the SRI format may be more convenient for some applications.

## Time
Time parameters are in the `Time` group.  This includes the time array expressed in different convenient units.  The time array contains the start time and end time of each integration period.  If a single time stamp needs to be assigned to each record, it is often convencient to use either the start of the integration period or the midpoint.
#### Calculate Midpoint
time_mid = np.mean(time, axis=1)

The easiest way to get datetime objects from the time arrays is by using the unix time array, and using either the numpy or datetime modules convert to datetime objects.  Unix time is counted as seconds since midnight on January 1, 1970.
#### Convert unix time to datetime
time = utime.astype('datetime64[s]')
time = [dt.datetime.utcfromtimestamp(ut) for ut in utime]
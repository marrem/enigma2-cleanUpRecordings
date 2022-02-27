# cleanUpRecordings

Script to clean recordings from OpenATV (Enigma2) STB recordings dir.
Recordings are removed oldest (based on lexical sort) first, untill
at least min_space is free on hd device.

Perl on OpenATV (`opkg` package) is rather limited (no (even core) modules
present apart from strict, warnings and Config. So everything has to 
be done in a rather DIY basic way.

Seems that every `facility.severity` is being forwarded to remote syslogd
by `logger`. So `system('logger', ....` should be enough.



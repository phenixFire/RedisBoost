Release Notes
==============
1.5.5
--------------
- fixed pipeline issue with big amount of commands: pipeline failed to process all pipelined commands 
(e.g. more than 10000 commands in pipeline)
- clarified pubsub ReadMessageAsync command. If command is called without filter, then all errors and unknown packets are 
returned to client without exceptions thrown. If ReadMessageAsync is called with filter, then exception is thrown if
error occured or unknown packet was received. So ReadMessageAsync without filter is guaranteed to be exceptionless.
- minor fixes and redesign

1.5.4
--------------
- project moved to .NET40
- updates accumulated since 1.3.5
- minor fixes

1.3.5
--------------
- serialization capability added
- pipelining support added
- MOVE, OBJECT, SORT, BITOP, SETBIT, GETBIT, MIGRATE, HINCRBYFLOAT, INCRBYFLOAT commands support added
- Supports whole set of Redis 2.6 commands (only some Server commands are eliminated)

1.1.2
--------------
- clients pool support added

1.1.0
--------------
- initial version. Supports almost whole Redis 2.6 command set.



This application was created as part of an event at the Charleston, SC
Unix Users' Group (primarily a Linux Users' Group). The task was to
create an application that would load a set of text documents and then
use parallel processing to count the words in each file.

At the time I was working as a C# developer for a local game studio and
offered to create the application using C# to be run under the Mono
(OSS .Net implementation) framework. In 2014, Microsoft had not yet
made their official .Net runtime available for Linux.

Interestingly enough, the .Net runtime will automatically determine if
parallel tasks are more efficiently run synchronously. Even though the
application is written using parallel task semantics, the output defintely
appeared to run synchronously. Splitting a string into "words" isn't
exactly a heavy processing task.

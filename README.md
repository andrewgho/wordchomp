wordchomp - given set of letters, generate sets of words that use them all
==========================================================================

This program takes a set of letters, and tries to generate all sets of
words (according to a dictionary file) which use all of the letters in
the set. For example, if you have a dozen Scrabble® tiles on your desk,
and you want to spell words with them rather than have them scattered
haphazardly about, you can use this program to figure out what words to
spell out, without leaving any letters left over.

The program is very inefficient for large letter sets, for example, for
finding pangrams for an entire alphabet.

Install
-------

This requires the `multimap` Ruby gem, which allows for hashes with
multiple values for the same key. The easiest installation mechanism is:

    bundle install
    bundle exec wordchomp example

The program also requires a dictionary, with one word per line. On Unix
hosts, you can find a dictionary file at `/usr/share/dict/words` (or, on
some older systems, `/usr/dict/words`). An unofficial copy of the
Official Scrabble® Player's Dictionary, 3rd Edition, is included in the
file `ospd3.txt`.

Author
------

Andrew Ho (<andrew@zeuscat.com>)

License
-------

    Copyright (c) 2013, Andrew Ho
    All rights reserved.
    
    Redistribution and use in source and binary forms, with or without
    modification, are permitted provided that the following conditions
    are met:
    
    1. Redistributions of source code must retain the above copyright
       notice, this list of conditions and the following disclaimer.
    
    2. Redistributions in binary form must reproduce the above copyright
       notice, this list of conditions and the following disclaimer in the
       documentation and/or other materials provided with the distribution.
    
    3. Neither the name of Andrew Ho nor the names of its contributors may
       be used to endorse or promote products derived from this software
       without specific prior written permission.
    
    THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS
    IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
    TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A
    PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
    HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
    SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED
    TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR
    PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
    LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
    NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
    SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.

The name _Scrabble_ is a trademark of Hasbro, Inc.

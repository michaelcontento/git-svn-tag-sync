Configure
---------

Simple git post-receive hook to sync new tags into a SVN repository.
Git configuration settings we need (or this hook refuse to do anything!):
      
* __svntagsync.auth.user__
    * The user used for all svn commands         
* __svntagsync.auth.pass__
    * The password used for all svn commands        
* __svntagsync.tempdir__
    * Temporary directory where we do all the work       
* __svntagsync.tagurl__
    * The url to the tag directory of your SVN project.
    * In the most cases that should be something like http://svn.server/tags/

Install
-------

* Copy the content of this into (.git/)hooks/post-recieve
* Mark the hook as executable: chmod +x (.git/)hooks/post-receive
* Configure the hook via git config (see below for details)


License
-------

    Copyright 2009-2010 Michael Contento <michaelcontento@gmail.com>

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

# Overview

This is a repository to house an implementation for converting query plans between
Substrait and Velox. This is in a stand-alone repository because the code in the
[Velox repository][repo-velox] did not have a maintainer and to make the use of velox
easier via substrait (independent of the [Gluten project][repo-gluten]).


<!-- resources -->
[repo-velox]:  https://github.com/facebookincubator/velox/
[repo-gluten]: https://github.com/oap-project/gluten/

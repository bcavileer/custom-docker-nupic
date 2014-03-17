my custom docker-nupic
============

Please see https://github.com/numenta/docker-nupic for official repository.

A Dockerfile for building a [NuPIC][1] image. 

Run the Python unit tests:

    docker run nupic /bin/bash -c "cd /usr/bin/nta/eng/;./bin/run_tests.sh"

Run the C++ tests:

    docker run nupic /bin/bash -c "/usr/bin/nta/eng/bin/htmtest"
    socker run nupic /bin/bash -c "/usr/bin/nta/eng/bin/testeverything"

Run hotgym example:

    docker run nupic /bin/bash -c "python /usr/local/src/nupic/examples/opf/clients/hotgym/hotgym.py"
    docker run nupic /bin/bash -c "python /usr/local/src/nupic/examples/opf/bin/OpfRunExperiment.py /usr/local/src/nupic/examples/opf/experiments/multistep/hotgym/"

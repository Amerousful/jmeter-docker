# jmeter-docker

https://hub.docker.com/r/amerousful/jmeter


Run: `docker run --name=${name} --volume /absolute/path/to/dir/no/trailing/slash:/jmeter_sample amerousful/jmeter -n -t /jmeter_sample/${suiteName}.jmx -l /jmeter_sample/result_${name}.jtl -j /jmeter_sample/jmeter_${name}.log -e -o /jmeter_sample/report_${name}`

Stop: `docker exec ${name} bash -c '${pwd}/bin/stoptest.sh' && docker stop ${name}`

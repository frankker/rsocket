# rsocket

Note:
1.) Download the rsc client from https://github.com/making/rsc (tested with 0.9.1)

2.) Command with authentication:
java -jar rsc.jar --debug --request --data "{\"origin\":\"Client\",\"interaction\":\"Request\"}" --route request-response tcp://localhost:7000 --sm simple:user:pass --smmt message/x.rsocket.authentication.v0

(for channel interaction, duration setting can be changed by request streaming)
java -jar rsc.jar --debug --channel --data - --route channel tcp://localhost:7000 --sm simple:user:pass --smmt message/x.rsocket.authentication.v0

Telive receivers with UDP transport and XMLRPC control, and helper files:

../kill_wrapper - a script to run an application and kill it when  ^C is
pressed. takes the command to be ran as argument, 
for example ../kill_wrapper ./telive_6ch_gr38_udp_xmlrpc_headless.py

telive_1ch_gr38_udp_xmlrpc_headless.grc - headless 1 channel receiver grc
script

telive_1ch_gr38_udp_xmlrpc_headless.py -
telive_1ch_gr38_udp_xmlrpc_headless.grc compiled to a python script via
gnuradio companion

telive_1ch_gr38_udp_xmlrpc_headless_slow.grc - headless 1 channel receiver grc
script with 256ks/s sammple rate for low cpu machines

telive_1ch_gr38_udp_xmlrpc_headless_slow.py -
telive_1ch_gr38_udp_xmlrpc_headless_slow.grc  compiled to a python script via
gnuradio companion


telive_6ch_gr38_udp_xmlrpc_headless.grc - headless 6 channel receiver grc
script 

telive_6ch_gr38_udp_xmlrpc_headless.py -
telive_6ch_gr38_udp_xmlrpc_headless.grc compiled to a python script via
gnuradio companion

NOTE: gnuradio-companion 3.8.1.0 (and potentially other versions) expects an outdated SimpleXMLRPCServer, if you're having issues running with gnuradio-companion, try running the pre-compiled scripts with python. To fix newly compiled scripts; replace "import SimpleXMLRPCServer" with "from xmlrpc.server import SimpleXMLRPCServer", and replace "SimpleXMLRPCServer.SimpleXMLRPCServer()" with "SimpleXMLRPCServer()" --adryd


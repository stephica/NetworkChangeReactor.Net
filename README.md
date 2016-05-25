# Network Change Reactor
A windows service that "Reacts" to network connection changes and then performs the pre-configured tasks.
For the time being, on detecting a network, it only opens the applications specified in the configuration

E.g. let's say your company's Intranet is accessible only from your office network.
This can thus tell the service that you have checked into the office and hence automatically kick start some applications for me e.g MS Outlook with which you start you day

#How to install
1. Build the installer project. 
2. Run the setup and install. 
3. After installing you will need to start the service 'NetworkReactor' manually by first running "services.msc" in run prompt.
4. Just make sure that the service is run with Local System account.

#Usage
1. In the installation folder open ReactorService.exe.config file.
2. Change the value of HOST_TO_CHECK attribute to a specific host name or IP address
that is going to be reachable from the changed network state.
3. Change the value of APPS_TO_START to semi-colon separated executables path



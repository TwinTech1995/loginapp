Step 1: Test port forwarding manually by running the command
(kubectl port-forward service/loginapp-service 18080:8080 --address 127.0.0.1)

Keep this window open. You should see:
Forwarding from 127.0.0.1:18080 -> 8080

Step 2: Test the application from another CMD window by running the command
(curl.exe -i --connect-timeout 5 http://127.0.0.1:18080/)

Step 3: Copy the URL and open it in new window to get the application
(http://127.0.0.1:18080/)

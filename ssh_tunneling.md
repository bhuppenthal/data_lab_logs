# SSH Tunneling Quick Explanation
[SSH Tunneling Reference](https://www.ssh.com/academy/ssh/tunneling-example)

Connect to the server using the local port forwarding option. This tunnels connections on port 6060 on your machine to port 8081 of the remote machine.
```
ssh -L 6060:localhost:8081 [remote_machine]
```

Once connected to the remote machine, provide the specified port as follows:
```
jupyter notebook --no-browser --port=8081
```

On your local machine, you can navigate to localhost:6060 to access the running notebook instance.

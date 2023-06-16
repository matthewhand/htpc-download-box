# Project Update

## Task: Connect to the server and execute commands

We connected to the server using the alias 'master'. The following commands were executed using nohup and ensuring unique output files:

1. `nohup sudo usermod -a -G microk8s chatgpt > nohup_usermod.out 2>&1; if [ $? -ne 0 ]; then cat nohup_usermod.out; fi; du -s nohup_usermod.out`
2. `nohup sudo chown -R chatgpt ~/.kube > nohup_chown.out 2>&1; if [ $? -ne 0 ]; then cat nohup_chown.out; fi; du -s nohup_chown.out`
3. `nohup newgrp microk8s > nohup_newgrp.out 2>&1; if [ $? -ne 0 ]; then cat nohup_newgrp.out; fi; du -s nohup_newgrp.out`

After executing the commands, we did some research on the current activity using WebPilot. The research provided insights into the process of creating a MicroK8s cluster and adding nodes to it. It also highlighted the importance of ensuring that the nodes have the correct time for inter-node communication to work.

We then read and deleted all nohup output files. The output files did not provide any output, indicating that the commands were executed successfully.

## Next Steps

The next step is to verify that the changes have taken effect and that the worker nodes can now join the master cluster. This will involve executing the join command on the worker nodes and checking the status of the nodes.
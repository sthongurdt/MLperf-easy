# Automatic Test Execution

Run the oar_exec.sh script, which requires three arguments. This script allocates resources using three arguments: the first argument defines the cluster where the test will be deployed, and the second and third arguments define the framework and model.
```
chmod +x oar_exec. sh exec_docker_onnx_mob.sh exec_docker_onnx_res.sh exec_docker_tf_mob.sh exec_docker_tf_res.sh
```
Example:
```
./oar_exec.sh taurus onnx mob
```

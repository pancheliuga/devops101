## Kubernetes Plugin: Resource Usage Statistics

This Kubernetes plugin allows you to retrieve resource usage statistics from a Kubernetes cluster and display them on the console. Follow the steps below to use the plugin:

1. **Prerequisites:**

   - Make sure you have `kubectl` installed and configured to connect to your Kubernetes cluster. You can refer to the Kubernetes documentation for installation instructions: [Install and Set Up kubectl](https://kubernetes.io/docs/tasks/tools/install-kubectl/).

2. **Download the Script:**

   - Download the script file named `kubeplugin` from the repository or source where it is available.

3. **Set Execution Permissions:**

   - Make the script executable by running the following command:

     ```shell
     $ chmod +x kubeplugin
     ```

4. **Usage Syntax:**

   - The script can be executed using the following syntax:

     ```shell
     $ ./kubeplugin RESOURCE_TYPE NAMESPACE
     ```

5. **Replace Arguments:**

   - Replace the `RESOURCE_TYPE` argument with the type of resource you want to retrieve usage statistics for. Examples include `pods`, `deployments`, `services`, etc.
   - Replace the `NAMESPACE` argument with the namespace in which the resources are located.

6. **Execute the Plugin:**

   - Run the script as a Kubernetes plugin by executing the following command:

     ```shell
     $ ./kubeplugin RESOURCE_TYPE NAMESPACE
     ```

   - The script will retrieve the resource usage statistics from the specified namespace and display them on the console.

7. **Review the Output:**

   - The output will show the resource statistics in the following format:

     ```
     Resource: [resource type], Namespace: [namespace], Name: [name], CPU: [CPU usage], Memory: [memory usage]
     ```

8. **Repeat as Needed:**

   - You can repeat the execution of the script with different `RESOURCE_TYPE` and `NAMESPACE` values to retrieve resource usage statistics for various resources within different namespaces.

That's it! You have successfully used the Kubernetes plugin script to retrieve resource usage statistics from your Kubernetes cluster.

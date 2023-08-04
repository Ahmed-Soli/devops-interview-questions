# Those are 50 Questions I was asked during a devops internship interview
1. **Question**: What is your main operating system?

   **Answer**: Windows.

2. **Question**: What are the differences between Windows and Linux?

   **Answer**: Windows is developed by Microsoft and is mainly used on personal computers, while Linux is an open-source operating system available in various distributions and widely used on servers and other devices.

3. **Question**: Define the Kernel.

   **Answer**: The Kernel is the core component of an operating system that manages system resources, handles communication between hardware and software, and provides essential services to the operating system.

4. **Question**: Explain what the Shell is.

   **Answer**: The Shell is a command-line interface that allows users to interact with the operating system by typing commands. It interprets and executes these commands to perform various tasks.

5. **Question**: What are the types of Shells?

   **Answer**: There are different types of shells, such as Bash (Bourne Again SHell), C shell (csh), Z shell (zsh), and more, each with its unique features and capabilities.

6. **Question**: How can you list the processes in the system?

   **Answer**: To list the processes in the system, you can use the "ps" command in the terminal.

7. **Question**: How do you kill a process?

   **Answer**: To kill a process, you can use the "kill" command followed by the process ID (PID) of the process you want to terminate.

8. **Question**: What is the signal of Kill and what's its number?

   **Answer**: The signal of "Kill" is SIGKILL, and its number is 9.

9. **Question**: How can you check the CPU usage?

   **Answer**: To check the CPU usage, you can use the "top" command or "htop" command in the terminal.

10. **Question**: How can you check the Memory usage?

    **Answer**: To check the Memory usage, you can use the "free" command in the terminal.

11. **Question**: How can you know the free and used disk space?

    **Answer**: To know the free and used disk space, you can use the "df" command in the terminal.

12. **Question**: Define permissions.

    **Answer**: Permissions in a file system define who can read, write, and execute files and directories.

13. **Question**: How do you change the permission of a file?

    **Answer**: To change the permission of a file, you can use the "chmod" command followed by the desired permission settings.

14. **Question**: What is the sticky bit?

    **Answer**: The sticky bit is a special permission that can be set on a directory. It allows only the file's owner to delete or rename their files within that directory, even if other users have write access to it.

15. **Question**: How can you know the status of a service?

    **Answer**: To know the status of a service, you can use service management commands specific to your operating system, such as "systemctl status" on Linux.

16. **Question**: How do you access a server on the cloud?

    **Answer**: To access a server on the cloud, you typically use SSH (Secure Shell) to establish a secure remote connection.

17. **Question**: What is the port used with SSH?

    **Answer**: The default port used with SSH is 22.

18. **Question**: Can you change the SSH port?

    **Answer**: Yes, you can change the SSH port by modifying the SSH server configuration file (sshd_config) and restarting the SSH service.

19. **Question**: What is the port of HTTP?

    **Answer**: The port of HTTP is 80.

20. **Question**: What is the port of HTTPS?

    **Answer**: The port of HTTPS is 443.

21. **Question**: Can you use the HTTP port for HTTPS and vice versa?

    **Answer**: No, you cannot use the HTTP port for HTTPS and vice versa; they are different protocols with different port numbers.

22. **Question**: Define the OSI model.

    **Answer**: The OSI (Open Systems Interconnection) model is a conceptual framework that standardizes the functions of a telecommunication or computing system into seven abstraction layers.

23. **Question**: What are the layers of the OSI Model?

    **Answer**: The layers of the OSI model are: 1. Physical, 2. Data Link, 3. Network, 4. Transport, 5. Session, 6. Presentation, 7. Application.

24. **Question**: In which layer does SSH work?

    **Answer**: SSH works on the Application layer (Layer 7) of the OSI model.

25. **Question**: If Server A can't reach Server B, what are the steps to troubleshoot the issue?

    **Answer**: The troubleshooting steps would include: 
    1. Check network connectivity using the ping command.
    2. Verify the IP addresses and network configurations of both servers.
    3. Check firewall settings on both servers to ensure there are no blocking rules.
    4. Verify that the required services on both servers are running and accessible.
    5. Check if there are any routing or networking issues.

26. **Question**: What's ping?

    **Answer**: Ping is a network utility used to test the reachability of a host on an Internet Protocol (IP) network and to measure the round-trip time for packets sent from the source to the destination.

27. **Question**: In which layer does ping work?

    **Answer**: Ping works on the Network layer (Layer 3) of the OSI model.

28. **Question**: How would you check the running firewall on the system?

    **Answer**: To check the running firewall on the system, you can use the appropriate command depending on the firewall software in use. For example, on Linux, you can use "iptables" or "firewalld" commands.

29. **Question**: What is DNS?

    **Answer**: DNS (Domain Name System) is a system that translates domain names (e.g., www.example.com) into IP addresses, allowing users to access websites using human-readable names.

30. **Question**: What is VPN?

    **Answer**: VPN (Virtual Private Network) is a secure and encrypted network connection that allows users to access the internet or internal resources as if they were directly connected to the private network.

31. **Question**: Can you use more than one FROM statement in a Dockerfile?

    **Answer**: you can use more than one FROM statement in your dockerfile and this's called multi-stage builds
https://docs.docker.com/build/building/multi-stage/

32. **Question**: What is the difference between CMD and ENTRYPOINT in Dockerfile?

    **Answer**: CMD sets the default command and arguments for the container, which can be overridden when running the container. ENTRYPOINT specifies the executable that will run when the container starts and allows you to pass additional arguments.

33. **Question**: What is Docker-compose?

    **Answer**: Docker-compose is a tool used to define and manage multi-container Docker applications. It uses a YAML file to configure services, networks, and volumes, allowing you to run complex applications easily.

34

. **Question**: What is the difference between a POD and a Deployment in Kubernetes?

    **Answer**: In Kubernetes, a POD is the smallest deployable unit that represents a single instance of a running process in a cluster, while a Deployment is a higher-level object that manages the deployment and scaling of replicas of a POD.

35. **Question**: What is the difference between ReplicaSet and StatefulSet in Kubernetes?

    **Answer**: Both ReplicaSet and StatefulSet are Kubernetes controllers used to manage the number of replicated pods, but StatefulSet is specifically designed for stateful applications that require stable network identities and persistent storage.

36. **Question**: What's a Service in Kubernetes?

    **Answer**: In Kubernetes, a Service is an abstraction that enables access to a set of pods. It provides a stable IP address and DNS name for the pods, allowing other applications to communicate with them.

37. **Question**: What are the Types of Services in Kubernetes?

    **Answer**: The types of Services in Kubernetes are ClusterIP, NodePort, LoadBalancer, and ExternalName.

38. **Summary**: ClusterIP is the default type for services in Kubernetes, used for internal communication between different components of an application. NodePort is used when you need to access the service externally, but it is not recommended for production environments. LoadBalancer is suitable for production environments when you need to expose a service to the public internet. ExternalName is used to provide access to external services running outside the cluster.

39. **Question**: What do you know about Jenkins, and what did you do with it?

    **Answer**: Jenkins is an open-source automation server used to automate various parts of the software development process, including building, testing, and deploying applications. As an AI language model, I don't have personal experiences, but users can use Jenkins to set up Continuous Integration and Continuous Deployment (CI/CD) pipelines.

40. **Question**: What are the Steps of a CI/CD job in Jenkins?

    **Answer**: The steps of a CI/CD job in Jenkins typically include: 
    1. Code checkout from version control.
    2. Building the application.
    3. Running automated tests.
    4. Packaging the application.
    5. Deploying the application to a test/staging environment.
    6. Running additional tests (e.g., integration tests).
    7. Deploying the application to production.

41. **Question**: What is the meaning of publishing the code?

    **Answer**: Publishing the code means making the source code of a software project available to others, often by uploading it to a code repository or version control system accessible to the public.

42. **Question**: How is the application triggered in a CI/CD?

    **Answer**: In CI/CD, the application is triggered automatically whenever a code change is pushed to the version control repository or when a specific event occurs, such as a merge request or a pull request.

43. **Question**: Are you familiar with any Infrastructure as Code tools?

    **Answer**: Yes, I'm familiar with Infrastructure as Code (IaC) tools. They are used to manage and provision infrastructure using code and configuration files.

44. **Question**: What did you do with Terraform?

    **Answer**: Terraform is an IaC tool used for infrastructure provisioning and management across various cloud providers and services.

45. **Question**: In AWS, what is the difference between EBS and EFS?

    **Answer**: In AWS, EBS (Elastic Block Store) is a block-level storage service used to create and attach persistent block storage volumes to EC2 instances, while EFS (Elastic File System) is a scalable and fully managed file storage service that provides shared access to files for multiple EC2 instances.

46. **Question**: what is EKS cluster ?

    **Answer**: EKS (Elastic Kubernetes Service) is a managed Kubernetes service provided by AWS.

47. **Question**: Did you work with Ansible before?

    **Answer**:  I'm familiar with Ansible, an open-source automation tool for configuration management, application deployment, and task automation.

48. **Question**: Did you write any bash script before?

    **Answer**: yes.

49. **Question**: How to write a bash script to take input from the user?

    **Answer**: To write a bash script that takes input from the user, you can use the "read" command, like this:

    ```bash
    #!/bin/bash
    echo "Enter your name: "
    read name
    echo "Hello, $name!"
    ```

50. **Question**: How to write "hello" inside the first 10 files only, where you have 1000 files?

    **Answer**: To write "hello" inside the first 10 files out of 1000, you can use a loop in a bash script, assuming the files are named "file1", "file2", and so on:

    ```bash
    #!/bin/bash
    for ((i = 1; i <= 10; i++)); do
        echo "hello" > "file$i"
    done
    ```
OR
echo "hello" > "{1..10}"

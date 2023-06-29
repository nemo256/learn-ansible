<div align="center">

# `Ansible with VirtualBox`

</div>

## `Introduction`

Ansible is an open-source automation platform that simplifies the management and deployment of IT systems. It allows you to automate tasks such as configuration management, application deployment, and orchestration across a wide range of systems, including servers, networking devices, and cloud infrastructure.

Here is why ansible is widely used in infrastructure automation:

- **Agentless Architecture**: Ansible uses SSH or WinRM protocols to connect to remote systems, eliminating the need for installing agents on target machines. This makes it lightweight and easy to set up.

- **Declarative Language**: Ansible uses a human-readable language called YAML (Yet Another Markup Language) to define tasks, configurations, and playbooks. This makes it easy to write, understand, and maintain automation code.

- **Playbooks and Roles**: Ansible organizes automation tasks into playbooks, which are YAML files containing a set of instructions for managing systems. Playbooks can be divided into reusable and shareable units called roles, making it easier to structure and manage complex automation workflows.

- **Idempotent Execution**: Ansible ensures idempotent execution, meaning that tasks are only applied if necessary. This allows you to repeatedly run playbooks without causing unintended changes, reducing the risk of configuration drift.

- **Inventory Management**: Ansible uses inventory files to define the target systems on which tasks will be executed. These files can be organized into groups and can include variables to define specific configurations for different systems.

- **Modules and Plugins**: Ansible provides a vast collection of pre-built modules that abstract complex system operations. Modules can be used to perform tasks such as installing packages, managing files, executing commands, and more. Ansible also supports custom plugins to extend its functionality.

- **Integration and Extensibility**: Ansible integrates with various tools and technologies, allowing you to create comprehensive automation workflows. It can interact with cloud platforms, version control systems, monitoring tools, and more. Ansible can also be extended through custom modules and plugins.

- **Community and Ecosystem**: Ansible has a large and active community that contributes to its development, provides support, and shares modules and playbooks through the Ansible Galaxy repository. This vibrant ecosystem makes it easier to leverage existing automation solutions.

Overall, Ansible's simplicity, scalability, and flexibility make it a popular choice for automating IT infrastructure and streamlining repetitive tasks, enabling faster and more reliable deployments and system management.

## `Introduction to VirtualBox and Vagrant`

VirtualBox is a popular open-source virtualization platform that allows users to create and manage virtual machines (VMs) on their computers. It enables the installation and operation of multiple operating systems simultaneously, emulating a complete computer system within a host machine.

On the other hand, Vagrant is an open-source tool that simplifies the configuration and management of virtual machines (VMs) for development and testing environments. It provides a consistent and reproducible workflow for setting up and managing VMs across different platforms.

By combining VirtualBox, Vagrant, and Ansible, we can easily create and manage reproducible development environments. This allows for consistent configurations, streamlined setup processes, and efficient collaboration among team members. Additionally, Ansible's automation capabilities enhance the provisioning and configuration of the virtual machines created by Vagrant, making it easier to manage complex systems and ensure consistent deployments.

## `How is ansible useful`

Ansible allowed me to create 2 debian virtual machines using custom configurations such as the ressources I set (How much RAM, CPUs, custom MAC addresses...) and also custom tasks to create, modify and mount the 2 debian VMs.

I also used the inventory.ini (initialization file) to set the target hosts (their hostnames, IP addresses and other configuration options).

(See the other files I used as an example)

Here are some benefits of using ansible:

1. Ansible Playbook

2. Ansible Modules

3. VirtualBox CLI

4. Inventory Configuration

5. Task Definition

6. Execution

## `Advantages of using ansible`

Advantages of using Ansible for the specified task (creating local virtual machines on VirtualBox):

1. **Simplicity and ease of use**: Ansible uses YAML which is very simple and does not require extensive programming knowledge, making it accessible to both beginners and experienced users.

2. **Agentless architecture**: Ansible operates in an agentless manner, leveraging SSH connections to communicate with remote systems. This eliminates the need to install and manage agents on target hosts, simplifying the setup process.

3. **Idempotent and declarative**: Ansible ensures that the desired state of the system is achieved regardless of its current state. It only applies necessary changes, minimizing unintended consequences and allowing for easy system configuration management.

4. **Large community and vast ecosystem**: Ansible has a thriving community and extensive documentation, providing access to a wide range of pre-built modules, playbooks, and roles. This allows users to leverage existing solutions and share knowledge with the community.

## `Disadvantages of using ansible`

1. **Limited real-time interaction**: Ansible primarily focuses on configuration management and automation, which means it may not be the best choice for tasks that require real-time interaction or immediate feedback.

2. **Learning curve**: While Ansible is relatively easy to learn for simple tasks, more complex scenarios may require a deeper understanding of its advanced features, such as conditionals, loops, and templating.

3. **Dependencies**: Ansible depends on SSH or other remote access mechanisms to connect to and manage remote systems. This dependency may pose challenges in environments with strict security policies or limited connectivity.

4. **GUI**: Ansible is only used as TUI (terminal user interface) there is no GUI (graphical user interface). I may argue that this one is an advantage because for development purposes command line applications are usually sufficient.

I have not used terraform yet, but just from research I think that both ansible and terraform are widely used in infrastructure automation and choosing one of them depends heavily on the given task.

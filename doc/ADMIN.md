## Setting up the agent

In case you missed the post-install information, your Beszel Agent is listening on port __PORT__.

You should have your Beszel app's `+ Add System` window already opened. Specify that port in lieu of the default `45876`. Fill in the name, domain name or IP address of this monitored server, then click on `Add System`.

If you closed the `+ Add System` modal, you need to uninstall the agent and reinstall it again, as the Token is regenerated each time the Add System procedure is started.

## Additional configuration

The agent monitors some basic things out of the box, but you may need to add some configuration manually in its environment file.

To do so, add any tweaks in the `__DATA_DIR__/.env.local` file. Do not forget to restart the `__APP__` service afterwards.

### Additional disks

Refer to the upstream documentation to check the usage of `EXTRA_FILESYSTEMS`: <https://beszel.dev/guide/additional-disks#binary-agent>

### GPU monitoring

Check the upstream documentation at <https://beszel.dev/guide/gpu#gpu-monitoring> to configurations needed to tell the Agent to monitor your GPU. They depend on its brand, notably.

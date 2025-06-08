# Example project

This is an example project to show that firebase app hosting does not work with nx, pnpm and sveltekit

See
apps/svelte/apphosting.yaml

Try to fork this repo and setup firebase app hosting you will get the following error:

```
An error occurred in your rollout
generic::failed_precondition: Revision 'test-sveltekit-build-2025-06-08-000' is not ready and cannot serve traffic. The user-provided container failed to start and listen on the port defined provided by the PORT=8080 environment variable within the allocated timeout. This can happen when the container port is misconfigured or if the timeout is too short. The health check timeout can be extended. Logs for this revision might contain more information. Logs URL: https://console.cloud.google.com/logs/viewer?project=bilverdi-dev&resource=cloud_run_revision/service_name/test-sveltekit/revision_name/test-sveltekit-build-2025-06-08-000&advancedFilter=resource.type%3D%22cloud_run_revision%22%0Aresource.labels.service_name%3D%22test-sveltekit%22%0Aresource.labels.revision_name%3D%22test-sveltekit-build-2025-06-08-000%22 For more troubleshooting guidance, see https://cloud.google.com/run/docs/troubleshooting#container-failed-to-start
```

## Requirements.
Python 2.7 and later.

## Notes
Based on Kubernetes 1.1.3. Should be a fully functional python interface to the Kubernetes API. v1.json modified slightly to replace "type": "any" with "type": "string". Not fully tested but is working quite well to this point.

## Setuptools
You can install the bindings via [Setuptools](http://pypi.python.org/pypi/setuptools).

```sh
python setup.py install
```

Or you can install from Github via pip:

```sh
pip install git+https://github.com/mward29/python-k8sclient.git
```

To use the bindings, import the package:

```python
import swagger_client
```

## Manual Installation
If you do not wish to use setuptools, you can download the latest release.
Then, to use the bindings, import the package:

```python
import path.to.swagger_client
```

<<<<<<< HEAD
## Getting Started

TODO

## List of Functions

get_api_resources():

    get available resources

--
list_namespaced_component_status():

    list objects of kind ComponentStatus

--
read_namespaced_component_status( name,):

    read the specified ComponentStatus

--
list_endpoints():

    list or watch objects of kind Endpoints

--
list_event():

    list or watch objects of kind Event

--
list_limit_range():

    list or watch objects of kind LimitRange

--
list_namespaced_namespace():

    list or watch objects of kind Namespace

--
create_namespaced_namespace( body,):

    create a Namespace

--
deletecollection_namespaced_namespace():

    delete collection of Namespace

--
create_namespaced_binding( body, namespace,):

    create a Binding

--
list_namespaced_endpoints( namespace,):

    list or watch objects of kind Endpoints

--
create_namespaced_endpoints( body, namespace,):

    create a Endpoints

--
deletecollection_namespaced_endpoints( namespace,):

    delete collection of Endpoints

--
read_namespaced_endpoints( namespace, name,):

    read the specified Endpoints

--
replace_namespaced_endpoints( body, namespace, name,):

    replace the specified Endpoints

--
delete_namespaced_endpoints( body, namespace, name,):

    delete a Endpoints

--
patch_namespaced_endpoints( body, namespace, name,):

    partially update the specified Endpoints

--
list_namespaced_event( namespace,):

    list or watch objects of kind Event

--
create_namespaced_event( body, namespace,):

    create a Event

--
deletecollection_namespaced_event( namespace,):

    delete collection of Event

--
read_namespaced_event( namespace, name,):

    read the specified Event

--
replace_namespaced_event( body, namespace, name,):

    replace the specified Event

--
delete_namespaced_event( body, namespace, name,):

    delete a Event

--
patch_namespaced_event( body, namespace, name,):

    partially update the specified Event

--
list_namespaced_limit_range( namespace,):

    list or watch objects of kind LimitRange

--
create_namespaced_limit_range( body, namespace,):

    create a LimitRange

--
deletecollection_namespaced_limit_range( namespace,):

    delete collection of LimitRange

--
read_namespaced_limit_range( namespace, name,):

    read the specified LimitRange

--
replace_namespaced_limit_range( body, namespace, name,):

    replace the specified LimitRange

--
delete_namespaced_limit_range( body, namespace, name,):

    delete a LimitRange

--
patch_namespaced_limit_range( body, namespace, name,):

    partially update the specified LimitRange

--
list_namespaced_persistent_volume_claim( namespace,):

    list or watch objects of kind PersistentVolumeClaim

--
create_namespaced_persistent_volume_claim( body, namespace,):

    create a PersistentVolumeClaim

--
deletecollection_namespaced_persistent_volume_claim( namespace,):

    delete collection of PersistentVolumeClaim

--
read_namespaced_persistent_volume_claim( namespace, name,):

    read the specified PersistentVolumeClaim

--
replace_namespaced_persistent_volume_claim( body, namespace, name,):

    replace the specified PersistentVolumeClaim

--
delete_namespaced_persistent_volume_claim( body, namespace, name,):

    delete a PersistentVolumeClaim

--
patch_namespaced_persistent_volume_claim( body, namespace, name,):

    partially update the specified PersistentVolumeClaim

--
replace_namespaced_persistent_volume_claim_status( body, namespace, name,):

    replace status of the specified PersistentVolumeClaim

--
list_namespaced_pod( namespace,):

    list or watch objects of kind Pod

--
create_namespaced_pod( body, namespace,):

    create a Pod

--
deletecollection_namespaced_pod( namespace,):

    delete collection of Pod

--
read_namespaced_pod( namespace, name,):

    read the specified Pod

--
replace_namespaced_pod( body, namespace, name,):

    replace the specified Pod

--
delete_namespaced_pod( body, namespace, name,):

    delete a Pod

--
patch_namespaced_pod( body, namespace, name,):

    partially update the specified Pod

--
connect_get_namespaced_pod_attach( namespace, name,):

    connect GET requests to attach of Pod

--
connect_post_namespaced_pod_attach( namespace, name,):

    connect POST requests to attach of Pod

--
create_namespaced_binding_binding( body, namespace, name,):

    create binding of a Binding

--
connect_get_namespaced_pod_exec( namespace, name,):

    connect GET requests to exec of Pod

--
connect_post_namespaced_pod_exec( namespace, name,):

    connect POST requests to exec of Pod

--
read_namespaced_pod_log( namespace, name,):

    read log of the specified Pod

--
connect_get_namespaced_pod_portforward( namespace, name,):

    connect GET requests to portforward of Pod

--
connect_post_namespaced_pod_portforward( namespace, name,):

    connect POST requests to portforward of Pod

--
connect_get_namespaced_pod_proxy( namespace, name,):

    connect GET requests to proxy of Pod

--
connect_head_namespaced_pod_proxy( namespace, name,):

    connect HEAD requests to proxy of Pod

--
connect_put_namespaced_pod_proxy( namespace, name,):

    connect PUT requests to proxy of Pod

--
connect_post_namespaced_pod_proxy( namespace, name,):

    connect POST requests to proxy of Pod

--
connect_delete_namespaced_pod_proxy( namespace, name,):

    connect DELETE requests to proxy of Pod

--
connect_options_namespaced_pod_proxy( namespace, name,):

    connect OPTIONS requests to proxy of Pod

--
connect_get_namespaced_pod_proxy_1( namespace, name, path2,):

    connect GET requests to proxy of Pod

--
connect_head_namespaced_pod_proxy_2( namespace, name, path2,):

    connect HEAD requests to proxy of Pod

--
connect_put_namespaced_pod_proxy_3( namespace, name, path2,):

    connect PUT requests to proxy of Pod

--
connect_post_namespaced_pod_proxy_4( namespace, name, path2,):

    connect POST requests to proxy of Pod

--
connect_delete_namespaced_pod_proxy_5( namespace, name, path2,):

    connect DELETE requests to proxy of Pod

--
connect_options_namespaced_pod_proxy_6( namespace, name, path2,):

    connect OPTIONS requests to proxy of Pod

--
replace_namespaced_pod_status( body, namespace, name,):

    replace status of the specified Pod

--
list_namespaced_pod_template( namespace,):

    list or watch objects of kind PodTemplate

--
create_namespaced_pod_template( body, namespace,):

    create a PodTemplate

--
deletecollection_namespaced_pod_template( namespace,):

    delete collection of PodTemplate

--
read_namespaced_pod_template( namespace, name,):

    read the specified PodTemplate

--
replace_namespaced_pod_template( body, namespace, name,):

    replace the specified PodTemplate

--
delete_namespaced_pod_template( body, namespace, name,):

    delete a PodTemplate

--
patch_namespaced_pod_template( body, namespace, name,):

    partially update the specified PodTemplate

--
list_namespaced_replication_controller( namespace,):

    list or watch objects of kind ReplicationController

--
create_namespaced_replication_controller( body, namespace,):

    create a ReplicationController

--
deletecollection_namespaced_replication_controller( namespace,):

    delete collection of ReplicationController

--
read_namespaced_replication_controller( namespace, name,):

    read the specified ReplicationController

--
replace_namespaced_replication_controller( body, namespace, name,):

    replace the specified ReplicationController

--
delete_namespaced_replication_controller( body, namespace, name,):

    delete a ReplicationController

--
patch_namespaced_replication_controller( body, namespace, name,):

    partially update the specified ReplicationController

--
replace_namespaced_replication_controller_status( body, namespace, name,):

    replace status of the specified ReplicationController

--
list_namespaced_resource_quota( namespace,):

    list or watch objects of kind ResourceQuota

--
create_namespaced_resource_quota( body, namespace,):

    create a ResourceQuota

--
deletecollection_namespaced_resource_quota( namespace,):

    delete collection of ResourceQuota

--
read_namespaced_resource_quota( namespace, name,):

    read the specified ResourceQuota

--
replace_namespaced_resource_quota( body, namespace, name,):

    replace the specified ResourceQuota

--
delete_namespaced_resource_quota( body, namespace, name,):

    delete a ResourceQuota

--
patch_namespaced_resource_quota( body, namespace, name,):

    partially update the specified ResourceQuota

--
replace_namespaced_resource_quota_status( body, namespace, name,):

    replace status of the specified ResourceQuota

--
list_namespaced_secret( namespace,):

    list or watch objects of kind Secret

--
create_namespaced_secret( body, namespace,):

    create a Secret

--
deletecollection_namespaced_secret( namespace,):

    delete collection of Secret

--
read_namespaced_secret( namespace, name,):

    read the specified Secret

--
replace_namespaced_secret( body, namespace, name,):

    replace the specified Secret

--
delete_namespaced_secret( body, namespace, name,):

    delete a Secret

--
patch_namespaced_secret( body, namespace, name,):

    partially update the specified Secret

--
list_namespaced_service_account( namespace,):

    list or watch objects of kind ServiceAccount

--
create_namespaced_service_account( body, namespace,):

    create a ServiceAccount

--
deletecollection_namespaced_service_account( namespace,):

    delete collection of ServiceAccount

--
read_namespaced_service_account( namespace, name,):

    read the specified ServiceAccount

--
replace_namespaced_service_account( body, namespace, name,):

    replace the specified ServiceAccount

--
delete_namespaced_service_account( body, namespace, name,):

    delete a ServiceAccount

--
patch_namespaced_service_account( body, namespace, name,):

    partially update the specified ServiceAccount

--
list_namespaced_service( namespace,):

    list or watch objects of kind Service

--
create_namespaced_service( body, namespace,):

    create a Service

--
read_namespaced_service( namespace, name,):

    read the specified Service

--
replace_namespaced_service( body, namespace, name,):

    replace the specified Service

--
delete_namespaced_service( namespace, name,):

    delete a Service

--
patch_namespaced_service( body, namespace, name,):

    partially update the specified Service

--
read_namespaced_namespace( name,):

    read the specified Namespace

--
replace_namespaced_namespace( body, name,):

    replace the specified Namespace

--
delete_namespaced_namespace( body, name,):

    delete a Namespace

--
patch_namespaced_namespace( body, name,):

    partially update the specified Namespace

--
replace_namespaced_namespace_finalize( body, name,):

    replace finalize of the specified Namespace

--
replace_namespaced_namespace_status( body, name,):

    replace status of the specified Namespace

--
list_namespaced_node():

    list or watch objects of kind Node

--
create_namespaced_node( body,):

    create a Node

--
deletecollection_namespaced_node():

    delete collection of Node

--
read_namespaced_node( name,):

    read the specified Node

--
replace_namespaced_node( body, name,):

    replace the specified Node

--
delete_namespaced_node( body, name,):

    delete a Node

--
patch_namespaced_node( body, name,):

    partially update the specified Node

--
replace_namespaced_node_status( body, name,):

    replace status of the specified Node

--
list_persistent_volume_claim():

    list or watch objects of kind PersistentVolumeClaim

--
list_namespaced_persistent_volume():

    list or watch objects of kind PersistentVolume

--
create_namespaced_persistent_volume( body,):

    create a PersistentVolume

--
deletecollection_namespaced_persistent_volume():

    delete collection of PersistentVolume

--
read_namespaced_persistent_volume( name,):

    read the specified PersistentVolume

--
replace_namespaced_persistent_volume( body, name,):

    replace the specified PersistentVolume

--
delete_namespaced_persistent_volume( body, name,):

    delete a PersistentVolume

--
patch_namespaced_persistent_volume( body, name,):

    partially update the specified PersistentVolume

--
replace_namespaced_persistent_volume_status( body, name,):

    replace status of the specified PersistentVolume

--
list_pod():

    list or watch objects of kind Pod

--
list_pod_template():

    list or watch objects of kind PodTemplate

--
proxy_get_namespaced_pod( namespace, name,):

    proxy GET requests to Pod

--
proxy_head_namespaced_pod( namespace, name,):

    proxy HEAD requests to Pod

--
proxy_put_namespaced_pod( namespace, name,):

    proxy PUT requests to Pod

--
proxy_post_namespaced_pod( namespace, name,):

    proxy POST requests to Pod

--
proxy_delete_namespaced_pod( namespace, name,):

    proxy DELETE requests to Pod

--
proxy_options_namespaced_pod( namespace, name,):

    proxy OPTIONS requests to Pod

--
proxy_get_namespaced_pod_7( namespace, name, path,):

    proxy GET requests to Pod

--
proxy_head_namespaced_pod_8( namespace, name, path,):

    proxy HEAD requests to Pod

--
proxy_put_namespaced_pod_9( namespace, name, path,):

    proxy PUT requests to Pod

--
proxy_post_namespaced_pod_10( namespace, name, path,):

    proxy POST requests to Pod

--
proxy_delete_namespaced_pod_11( namespace, name, path,):

    proxy DELETE requests to Pod

--
proxy_options_namespaced_pod_12( namespace, name, path,):

    proxy OPTIONS requests to Pod

--
proxy_get_namespaced_service( namespace, name,):

    proxy GET requests to Service

--
proxy_head_namespaced_service( namespace, name,):

    proxy HEAD requests to Service

--
proxy_put_namespaced_service( namespace, name,):

    proxy PUT requests to Service

--
proxy_post_namespaced_service( namespace, name,):

    proxy POST requests to Service

--
proxy_delete_namespaced_service( namespace, name,):

    proxy DELETE requests to Service

--
proxy_options_namespaced_service( namespace, name,):

    proxy OPTIONS requests to Service

--
proxy_get_namespaced_service_13( namespace, name, path,):

    proxy GET requests to Service

--
proxy_head_namespaced_service_14( namespace, name, path,):

    proxy HEAD requests to Service

--
proxy_put_namespaced_service_15( namespace, name, path,):

    proxy PUT requests to Service

--
proxy_post_namespaced_service_16( namespace, name, path,):

    proxy POST requests to Service

--
proxy_delete_namespaced_service_17( namespace, name, path,):

    proxy DELETE requests to Service

--
proxy_options_namespaced_service_18( namespace, name, path,):

    proxy OPTIONS requests to Service

--
proxy_get_namespaced_node( name,):

    proxy GET requests to Node

--
proxy_head_namespaced_node( name,):

    proxy HEAD requests to Node

--
proxy_put_namespaced_node( name,):

    proxy PUT requests to Node

--
proxy_post_namespaced_node( name,):

    proxy POST requests to Node

--
proxy_delete_namespaced_node( name,):

    proxy DELETE requests to Node

--
proxy_options_namespaced_node( name,):

    proxy OPTIONS requests to Node

--
proxy_get_namespaced_node_19( name, path,):

    proxy GET requests to Node

--
proxy_head_namespaced_node_20( name, path,):

    proxy HEAD requests to Node

--
proxy_put_namespaced_node_21( name, path,):

    proxy PUT requests to Node

--
proxy_post_namespaced_node_22( name, path,):

    proxy POST requests to Node

--
proxy_delete_namespaced_node_23( name, path,):

    proxy DELETE requests to Node

--
proxy_options_namespaced_node_24( name, path,):

    proxy OPTIONS requests to Node

--
list_replication_controller():

    list or watch objects of kind ReplicationController

--
list_resource_quota():

    list or watch objects of kind ResourceQuota

--
list_secret():

    list or watch objects of kind Secret

--
list_service_account():

    list or watch objects of kind ServiceAccount

--
list_service():

    list or watch objects of kind Service

--
watch_endpoints_list():

    watch individual changes to a list of Endpoints

--
watch_event_list():

    watch individual changes to a list of Event

--
watch_limit_range_list():

    watch individual changes to a list of LimitRange

--
watch_namespaced_namespace_list():

    watch individual changes to a list of Namespace

--
watch_namespaced_endpoints_list( namespace,):

    watch individual changes to a list of Endpoints

--
watch_namespaced_endpoints( namespace, name,):

    watch changes to an object of kind Endpoints

--
watch_namespaced_event_list( namespace,):

    watch individual changes to a list of Event

--
watch_namespaced_event( namespace, name,):

    watch changes to an object of kind Event

--
watch_namespaced_limit_range_list( namespace,):

    watch individual changes to a list of LimitRange

--
watch_namespaced_limit_range( namespace, name,):

    watch changes to an object of kind LimitRange

--
watch_namespaced_persistent_volume_claim_list( namespace,):

    watch individual changes to a list of PersistentVolumeClaim

--
watch_namespaced_persistent_volume_claim( namespace, name,):

    watch changes to an object of kind PersistentVolumeClaim

--
watch_namespaced_pod_list( namespace,):

    watch individual changes to a list of Pod

--
watch_namespaced_pod( namespace, name,):

    watch changes to an object of kind Pod

--
watch_namespaced_pod_template_list( namespace,):

    watch individual changes to a list of PodTemplate

--
watch_namespaced_pod_template( namespace, name,):

    watch changes to an object of kind PodTemplate

--
watch_namespaced_replication_controller_list( namespace,):

    watch individual changes to a list of ReplicationController

--
watch_namespaced_replication_controller( namespace, name,):

    watch changes to an object of kind ReplicationController

--
watch_namespaced_resource_quota_list( namespace,):

    watch individual changes to a list of ResourceQuota

--
watch_namespaced_resource_quota( namespace, name,):

    watch changes to an object of kind ResourceQuota

--
watch_namespaced_secret_list( namespace,):

    watch individual changes to a list of Secret

--
watch_namespaced_secret( namespace, name,):

    watch changes to an object of kind Secret

--
watch_namespaced_service_account_list( namespace,):

    watch individual changes to a list of ServiceAccount

--
watch_namespaced_service_account( namespace, name,):

    watch changes to an object of kind ServiceAccount

--
watch_namespaced_service_list( namespace,):

    watch individual changes to a list of Service

--
watch_namespaced_service( namespace, name,):

    watch changes to an object of kind Service

--
watch_namespaced_namespace( name,):

    watch changes to an object of kind Namespace

--
watch_namespaced_node_list():

    watch individual changes to a list of Node

--
watch_namespaced_node( name,):

    watch changes to an object of kind Node

--
watch_persistent_volume_claim_list():

    watch individual changes to a list of PersistentVolumeClaim

--
watch_namespaced_persistent_volume_list():

    watch individual changes to a list of PersistentVolume

--
watch_namespaced_persistent_volume( name,):

    watch changes to an object of kind PersistentVolume

--
watch_pod_list():

    watch individual changes to a list of Pod

--
watch_pod_template_list():

    watch individual changes to a list of PodTemplate

--
watch_replication_controller_list():

    watch individual changes to a list of ReplicationController

--
watch_resource_quota_list():

    watch individual changes to a list of ResourceQuota

--
watch_secret_list():

    watch individual changes to a list of Secret

--
watch_service_account_list():

    watch individual changes to a list of ServiceAccount

--
watch_service_list():

    watch individual changes to a list of Service


=======
>>>>>>> c06abede3d3fad7ec27bd9fff0a222a7dcc68a92
## Tests

(Please make sure you have [virtualenv](http://docs.python-guide.org/en/latest/dev/virtualenvs/) installed)

 Execute the following command to run the tests in the current Python (v2 or v3) environment:

```sh
$ make test
[... magically installs dependencies and runs tests on your virtualenv]
Ran 7 tests in 19.289s

OK
```
or

```
$ mvn integration-test -rf :PythonPetstoreClientTests
Using 2195432783 as seed
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time: 37.594 s
[INFO] Finished at: 2015-05-16T18:00:35+08:00
[INFO] Final Memory: 11M/156M
[INFO] ------------------------------------------------------------------------
```
If you want to run the tests in all the python platforms:

```sh
$ make test-all
[... tox creates a virtualenv for every platform and runs tests inside of each]
  py27: commands succeeded
  py34: commands succeeded
  congratulations :)
```

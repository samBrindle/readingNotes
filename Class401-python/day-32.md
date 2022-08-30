# Reading - Permissions and Postgresql
## DRF Permissions
"Authentication or identification by itself is not usually sufficient to gain access to information or code. For that, the entity requesting access must have authorization."
* Authentication and throttling come together to determine which permissions a user should be granted/denied
* Permission checks are always fun at the very start of view, before code is ran
* Utilize request.user and request.auth properties to check permissions

### How permissions are determined
* REST permissions are defined as a list of permission classes
* On load, each permission in the list is checked
  * If any check fails an `excepetions.PermissionDenied` or `exceptions.NotAuthenticated` excpetion will be raised
* If exception is raised, main will not run

### Object Level Permissions
* Object level permissions are used to check if users have access to particular objects, model instances
* You need to filter the queryset appropriately to ensure users only get access to instances they are allowed

### Setting the permisison policy
* Default permissions are set using `DEFAULT_PERMISSION_CLASSES`
  * if not specified, the settings default to unrestricted access
* You can also set authentication on a per-view/per-viewset basis with `APIView` class
* `@api_view` decorator is another option for function based views

### API Reference
* AllowAny
* IsAuthenticated
* IsAdminUser
* IsAuthenticatedOrReadOnly
* DjangoModelPermissions
* DjangoModelPermissionsOrAnonReadOnly
* DjangoObjectPermissions

<!-- YAML
added: v8.5.0
-->
```C
NAPI_EXTERN napi_status napi_run_script(napi_env env,
                                        napi_value script,
                                        napi_value* result);
```

- `[in] env`: The environment that the API is invoked under.
- `[in] script`: A JavaScript string containing the script to execute.
- `[out] result`: The value resulting from having executed the script.

[Promises]: #n_api_promises
[Simple Asynchronous Operations]: #n_api_simple_asynchronous_operations
[Custom Asynchronous Operations]: #n_api_custom_asynchronous_operations
[Basic N-API Data Types]: #n_api_basic_n_api_data_types
[ECMAScript Language Specification]: https://tc39.github.io/ecma262/
[Error Handling]: #n_api_error_handling
[Module Registration]: #n_api_module_registration
[Native Abstractions for Node.js]: https://github.com/nodejs/nan
[Object Lifetime Management]: #n_api_object_lifetime_management
[Object Wrap]: #n_api_object_wrap
[Script Execution]: #n_api_script_execution
[Section 9.1.6]: https://tc39.github.io/ecma262/#sec-ordinary-object-internal-methods-and-internal-slots-defineownproperty-p-desc
[Section 12.5.5]: https://tc39.github.io/ecma262/#sec-typeof-operator
[Section 24.3]: https://tc39.github.io/ecma262/#sec-dataview-objects
[Section 25.4]: https://tc39.github.io/ecma262/#sec-promise-objects
[Working with JavaScript Functions]: #n_api_working_with_javascript_functions
[Working with JavaScript Properties]: #n_api_working_with_javascript_properties
[Working with JavaScript Values]: #n_api_working_with_javascript_values
[Working with JavaScript Values - Abstract Operations]: #n_api_working_with_javascript_values_abstract_operations

[`napi_cancel_async_work`]: #n_api_napi_cancel_async_work
[`napi_close_escapable_handle_scope`]: #n_api_napi_close_escapable_handle_scope
[`napi_close_handle_scope`]: #n_api_napi_close_handle_scope
[`napi_create_async_work`]: #n_api_napi_create_async_work
[`napi_create_error`]: #n_api_napi_create_error
[`napi_create_external_arraybuffer`]: #n_api_napi_create_external_arraybuffer
[`napi_create_range_error`]: #n_api_napi_create_range_error
[`napi_create_reference`]: #n_api_napi_create_reference
[`napi_create_type_error`]: #n_api_napi_create_type_error
[`napi_delete_async_work`]: #n_api_napi_delete_async_work
[`napi_define_class`]: #n_api_napi_define_class
[`napi_delete_element`]: #n_api_napi_delete_element
[`napi_delete_property`]: #n_api_napi_delete_property
[`napi_delete_reference`]: #n_api_napi_delete_reference
[`napi_escape_handle`]: #n_api_napi_escape_handle
[`napi_get_array_length`]: #n_api_napi_get_array_length
[`napi_get_element`]: #n_api_napi_get_element
[`napi_get_property`]: #n_api_napi_get_property
[`napi_has_property`]: #n_api_napi_has_property
[`napi_has_own_property`]: #n_api_napi_has_own_property
[`napi_set_property`]: #n_api_napi_set_property
[`napi_get_reference_value`]: #n_api_napi_get_reference_value
[`napi_is_error`]: #n_api_napi_is_error
[`napi_is_exception_pending`]: #n_api_napi_is_exception_pending
[`napi_get_last_error_info`]: #n_api_napi_get_last_error_info
[`napi_get_and_clear_last_exception`]: #n_api_napi_get_and_clear_last_exception
[`napi_make_callback`]: #n_api_napi_make_callback
[`napi_open_escapable_handle_scope`]: #n_api_napi_open_escapable_handle_scope
[`napi_open_handle_scope`]: #n_api_napi_open_handle_scope
[`napi_property_descriptor`]: #n_api_napi_property_descriptor
[`napi_queue_async_work`]: #n_api_napi_queue_async_work
[`napi_reference_ref`]: #n_api_napi_reference_ref
[`napi_reference_unref`]: #n_api_napi_reference_unref
[`napi_throw`]: #n_api_napi_throw
[`napi_throw_error`]: #n_api_napi_throw_error
[`napi_throw_range_error`]: #n_api_napi_throw_range_error
[`napi_throw_type_error`]: #n_api_napi_throw_type_error
[`napi_unwrap`]: #n_api_napi_unwrap
[`napi_wrap`]: #n_api_napi_wrap

[`process.release`]: process.html#process_process_release
[`init` hooks]: async_hooks.html#async_hooks_init_asyncid_type_triggerasyncid_resource
[async_hooks `type`]: async_hooks.html#async_hooks_type

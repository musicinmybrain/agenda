test_task_source = files(
    'TestCase.vala',
    'TestTask.vala',
    'TestTaskMain.vala'
)

test_task_list_source = files(
    'TestCase.vala',
    'TestTaskList.vala',
    'TestTaskListMain.vala'
)

test_task_list_history_source = files(
    'TestCase.vala',
    'TestTaskListHistory.vala',
    'TestTaskListHistoryMain.vala'
)

task_test_bin = executable('test-task',
    test_task_source + agenda_model_sources,
    dependencies: agenda_deps,
    vala_args: vala_args,
    c_args: c_args,
)

task_list_test_bin = executable('test-task-list',
    test_task_list_source + agenda_model_sources,
    dependencies: agenda_deps,
    vala_args: vala_args,
    c_args: c_args,
)

task_list_history_test_bin = executable('test-task-list-history',
    test_task_list_history_source + agenda_model_sources,
    dependencies: agenda_deps,
    vala_args: vala_args,
    c_args: c_args,
)

test('test-task', task_test_bin)
test('test-task-list', task_list_test_bin)
test('test-task-list-history', task_list_history_test_bin)

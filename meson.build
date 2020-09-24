ucos3_deps = []
ucos3_inc = include_directories('Ports' / architecture / compiler, 'Source')
ucos3_src = files(
  'Source/os_cfg_app.c',
  'Source/os_core.c',
  'Source/os_dbg.c',
  'Source/os_flag.c',
  'Source/os_mem.c',
  'Source/os_msg.c',
  'Source/os_mutex.c',
  'Source/os_prio.c',
  'Source/os_q.c',
  'Source/os_sem.c',
  'Source/os_stat.c',
  'Source/os_task.c',
  'Source/os_tick.c',
  'Source/os_time.c',
  'Source/os_tmr.c',
  'Source/os_var.c',
)
if get_variable('default_configuration', false)
  ucos3_inc = [ucos3_inc, include_directories('Cfg/Template')]
  ucos3_src += files('Cfg/Template/os_app_hooks.c')
endif
subdir('Ports' / architecture)

运行方法
在10.1.0.106执行

python distribute.py --job_name=worker --ps_hosts=10.1.0.44:11111 --worker_hosts=10.1.0.44:22222,10.1.0.106:22223 --task_index=1

在10.1.0.44执行

python distribute.py --job_name=worker --ps_hosts=10.1.0.44:11111 --worker_hosts=10.1.0.44:22222,10.1.0.106:22223 --task_index=0

在10.1.0.44执行

python distribute.py --job_name=ps --ps_hosts=10.1.0.44:11111 --worker_hosts=10.1.0.44:22222,10.1.0.106:22223 --task_index=0
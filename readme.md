���з���
��10.1.0.106ִ��

python distribute.py --job_name=worker --ps_hosts=10.1.0.44:11111 --worker_hosts=10.1.0.44:22222,10.1.0.106:22223 --task_index=1

��10.1.0.44ִ��

python distribute.py --job_name=worker --ps_hosts=10.1.0.44:11111 --worker_hosts=10.1.0.44:22222,10.1.0.106:22223 --task_index=0

��10.1.0.44ִ��

python distribute.py --job_name=ps --ps_hosts=10.1.0.44:11111 --worker_hosts=10.1.0.44:22222,10.1.0.106:22223 --task_index=0
### How to use
1. Replace `172.17.0.1` in below command with your server IP address
   * https://github.com/ki4070ma/docker/blob/master/stf/docker-compose.yml

   ```
      command: stf local --public-ip 172.17.0.1 --provider-min-port 7400 --provider-max-port 7500 --adb-host adbd
   ```

2. `$cd /path/to/stf` and `$docker-compose up -d`

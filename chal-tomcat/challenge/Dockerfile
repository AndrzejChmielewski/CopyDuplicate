# Copyright 2020 Google LLC
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#     https://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
FROM duonghuuphuc/tomcat-8.5.32:latest

#RUN touch /error.log&& 
  #echo "tail -f /error.log" >> /run.sh
  
#VOLUME /tmp/
#VOLUME /etc/init.d/
#VOLUME /var/lib/mysql/
#VOLUME /var/log/apache2/
#VOLUME /var/www/
#VOLUME /var/lock/


VOLUME /usr/local/tomcat
RUN chmod -R 777 /usr/local/tomcat
COPY index.html /usr/local/tomcat/webapps/ROOT/

#CMD ["sh", "-c", "/run.sh"]
CMD ["catalina.sh", "run"]
#RUN /usr/sbin/useradd --no-create-home -u 1000 user

#COPY flag /
#COPY chal /home/user/

#FROM gcr.io/kctf-docker/challenge@sha256:0f7d757bcda470c3bbc063606335b915e03795d72ba1d8fdb6f0f9ff3757364f

#COPY --from=chroot / /chroot#

#COPY nsjail.cfg /home/user/

#CMD kctf_setup && \
 #   kctf_drop_privs \
 #   socat \
  #    TCP-LISTEN:1337,reuseaddr,fork \
 #     EXEC:"kctf_pow nsjail --config /home/user/nsjail.cfg -- /home/user/chal"
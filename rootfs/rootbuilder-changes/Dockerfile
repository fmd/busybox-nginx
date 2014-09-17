FROM progrium/rootbuilder
# Hehe, can't use sed
RUN sed '/menu "Networking applications"/a\source \"package\/nginx\/Config.in"' /tmp/buildroot/package/Config.in > tmpfile
RUN mv tmpfile /tmp/buildroot/package/Config.in
ADD ./package/nginx /tmp/buildroot/package/nginx

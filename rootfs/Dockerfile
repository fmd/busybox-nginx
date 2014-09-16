FROM progrium/rootbuilder
ADD ./config /tmp/buildroot/.config
ADD ./package /tmp/buildroot/package
RUN echo 'source "package/nginx/Config.in"' >> /tmp/buildroot/Config.in
RUN make oldconfig
RUN make --quiet

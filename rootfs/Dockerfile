FROM progrium/rootbuilder
ADD ./config /tmp/buildroot/.config
ADD ./package /tmp/buildroot/package
RUN make oldconfig
RUN make --quiet

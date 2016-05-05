FROM j24cape/perl
MAINTAINER NISHIZAKI Tadashi <j24cape@gmail.com>

RUN cpan-outdated -p | cpanm --notest > /tmp/cpanm-outdated.log 2>&1 \
    && cpanm --notest \
        Amon2 \
        Carton \
        Server::Starter \
      > /tmp/cpanm.log 2>&1 \
    && rm -fr /root/.cpanm /tmp/*

CMD ["perl", "-v"]

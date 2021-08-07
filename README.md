# Build
## With Docker

```bash
cp Firmware/variants/1_75mm_MK3S-EINSy10a-E3Dv6full.h Firmware/Configuration_prusa.h
docker image build . -f ./docker/Dockerfile -t build-fw
docker run --rm -v $PWD:/build build-fw
```

The built firmware file is output as `/lang/firmware.hex` 🙃

# Multi-Platform AWS Lambda Environment Image

This repository auto-builds a multi-platform (`x86_64`/`ARM64`) Docker image for the `provided.al2023` AWS Lambda environment.

The `provided.al2023` environment is the one intended for compiled code (C, C++, Rust, Go, etc.), or to use [Lambda Layers](https://docs.aws.amazon.com/lambda/latest/dg/chapter-layers.html) to modify.

## Usage

Container image path:

```text
ghcr.io/northwood-labs/lambda-provided-al2023:latest
```

## Issues

If you have an issue with this multi-platform Docker image, **DO NOT FILE AN ISSUE HERE**. Instead, [file an issue with AWS](https://github.com/aws/aws-lambda-base-images/tree/provided.al2023).

## Source

The Docker image is re-generated with AWS’ latest changes weekly on Saturday at 9:41am UTC.

<https://github.com/aws/aws-lambda-base-images/tree/provided.al2023>

### Doesn't AWS already provide these?

Yes. <https://gallery.ecr.aws/lambda/provided>

But they're broken.

```bash
docker pull public.ecr.aws/lambda/provided:al2023
Error response from daemon: failed to resolve reference "public.ecr.aws/lambda/provided:al2023": unexpected status from HEAD request to https://public.ecr.aws/v2/lambda/provided/manifests/al2023: 403 Forbidden
```

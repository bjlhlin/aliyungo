# AliyunGo: Go SDK for Aliyun Services

[![Build Status](https://travis-ci.org/bjlhlin/aliyungo.svg?branch=master)](https://travis-ci.org/bjlhlin/aliyungo) [![CircleCI](https://circleci.com/gh/bjlhlin/aliyungo.svg?style=svg)](https://circleci.com/gh/bjlhlin/aliyungo) [![Go Report Card](https://goreportcard.com/badge/github.com/bjlhlin/aliyungo)](https://goreportcard.com/report/github.com/bjlhlin/aliyungo)

This is an unofficial Go SDK for Aliyun services. You are welcome for contribution.

The official SDK for Aliyun services is published. Please visit https://github.com/aliyun/alibaba-cloud-sdk-go for details

## Package Structure

* cdn: [Content Delivery Network](https://help.aliyun.com/document_detail/27101.html)
* cms: [Cloud Monitor Service](https://help.aliyun.com/document_detail/28615.html)
* cs: [Container Service](https://help.aliyun.com/product/25972.html)
* dm: [Direct Mail](https://help.aliyun.com/document_detail/29414.html)
* dns: [DNS](https://help.aliyun.com/document_detail/dns/api-reference/summary.html)
* ecs: [Elastic Compute Service](https://help.aliyun.com/document_detail/ecs/open-api/summary.html)
* ess: [Auto Scaling](https://help.aliyun.com/document_detail/25857.html)
* mns: [Message Service](https://help.aliyun.com/document_detail/27414.html)
* mq: [Message Queue](https://help.aliyun.com/document_detail/29532.html)
* nas: [Network Attached Storage](https://help.aliyun.com/document_detail/27518.html)
* opensearch: [OpenSearch](https://help.aliyun.com/document_detail/29118.html)
* oss: [Open Storage Service](https://help.aliyun.com/document_detail/oss/api-reference/abstract.html)
* push: [Cloud Mobile Push](https://help.aliyun.com/document_detail/30049.html)
* rds: [Relational Database Service](https://help.aliyun.com/document_detail/26226.html)
* ram: [Resource Access Management](https://help.aliyun.com/document_detail/ram/ram-api-reference/intro/intro.html)
* slb: [Server Load Balancer](https://help.aliyun.com/document_detail/slb/api-reference/brief-introduction.html)
* sls: [Logging Service](https://help.aliyun.com/document_detail/sls/api/overview.html)
* sms: [Short Message Service](https://help.aliyun.com/product/44282.html)
* sts: [Security Token Service](https://help.aliyun.com/document_detail/28756.html)
* common: Common libary of Aliyun Go SDK
* util: Utility helpers

## Quick Start

```go
package main

import (
  "fmt"

	"github.com/bjlhlin/aliyungo/ecs"
)

const ACCESS_KEY_ID = "<YOUR_ID>"
const ACCESS_KEY_SECRET = "<****>"

func main() {
	client := ecs.NewClient(ACCESS_KEY_ID, ACCESS_KEY_SECRET)
	fmt.Print(client.DescribeRegions())
}

```

## Documentation

  * CDN: [https://godoc.org/github.com/bjlhlin/aliyungo/cdn](https://godoc.org/github.com/bjlhlin/aliyungo/cdn)[![GoDoc](https://godoc.org/github.com/bjlhlin/aliyungo/cdn?status.svg)](https://godoc.org/github.com/bjlhlin/aliyungo/cdn)
  * CMS: [https://godoc.org/github.com/bjlhlin/aliyungo/cms](https://godoc.org/github.com/bjlhlin/aliyungo/cms) [![GoDoc](https://godoc.org/github.com/bjlhlin/aliyungo/cms?status.svg)](https://godoc.org/github.com/bjlhlin/aliyungo/cms)
  * CS: [https://godoc.org/github.com/bjlhlin/aliyungo/cs](https://godoc.org/github.com/bjlhlin/aliyungo/cs) [![GoDoc](https://godoc.org/github.com/bjlhlin/aliyungo/cs?status.svg)](https://godoc.org/github.com/bjlhlin/aliyungo/cs)
  * DM: [https://godoc.org/github.com/bjlhlin/aliyungo/dm](https://godoc.org/github.com/bjlhlin/aliyungo/dm) [![GoDoc](https://godoc.org/github.com/bjlhlin/aliyungo/dm?status.svg)](https://godoc.org/github.com/bjlhlin/aliyungo/dm)
  * DNS: [https://godoc.org/github.com/bjlhlin/aliyungo/dns](https://godoc.org/github.com/bjlhlin/aliyungo/dns) [![GoDoc](https://godoc.org/github.com/bjlhlin/aliyungo/dns?status.svg)](https://godoc.org/github.com/bjlhlin/aliyungo/dns)
  * ECS: [https://godoc.org/github.com/bjlhlin/aliyungo/ecs](https://godoc.org/github.com/bjlhlin/aliyungo/ecs) [![GoDoc](https://godoc.org/github.com/bjlhlin/aliyungo/ecs?status.svg)](https://godoc.org/github.com/bjlhlin/aliyungo/ecs)
  * ESS: [https://godoc.org/github.com/bjlhlin/aliyungo/ess](https://godoc.org/github.com/bjlhlin/aliyungo/ess)[![GoDoc](https://godoc.org/github.com/bjlhlin/aliyungo/ess?status.svg)](https://godoc.org/github.com/bjlhlin/aliyungo/ess)
  * MNS: [https://godoc.org/github.com/bjlhlin/aliyungo/mns](https://godoc.org/github.com/bjlhlin/aliyungo/mns)[![GoDoc](https://godoc.org/github.com/bjlhlin/aliyungo/mns?status.svg)](https://godoc.org/github.com/bjlhlin/aliyungo/mns)
  * MQ: [https://godoc.org/github.com/bjlhlin/aliyungo/mq](https://godoc.org/github.com/bjlhlin/aliyungo/mq) [![GoDoc](https://godoc.org/github.com/bjlhlin/aliyungo/mq?status.svg)](https://godoc.org/github.com/bjlhlin/aliyungo/mq)
  * NAS: [https://godoc.org/github.com/bjlhlin/aliyungo/nas](https://godoc.org/github.com/bjlhlin/aliyungo/nas) [![GoDoc](https://godoc.org/github.com/bjlhlin/aliyungo/nas?status.svg)](https://godoc.org/github.com/bjlhlin/aliyungo/nas)
  * OPENSEARCH: [https://godoc.org/github.com/bjlhlin/aliyungo/opensearch](https://godoc.org/github.com/bjlhlin/aliyungo/opensearch) [![GoDoc](https://godoc.org/github.com/bjlhlin/aliyungo/opensearch?status.svg)](https://godoc.org/github.com/bjlhlin/aliyungo/opensearch)
  * OSS: [https://godoc.org/github.com/bjlhlin/aliyungo/oss](https://godoc.org/github.com/bjlhlin/aliyungo/oss) [![GoDoc](https://godoc.org/github.com/bjlhlin/aliyungo/oss?status.svg)](https://godoc.org/github.com/bjlhlin/aliyungo/oss)
  * PUSH: [https://godoc.org/github.com/bjlhlin/aliyungo/push](https://godoc.org/github.com/bjlhlin/aliyungo/push) [![GoDoc](https://godoc.org/github.com/bjlhlin/aliyungo/push?status.svg)](https://godoc.org/github.com/bjlhlin/aliyungo/push)
  * RAM: [https://godoc.org/github.com/bjlhlin/aliyungo/ram](https://godoc.org/github.com/bjlhlin/aliyungo/ram) [![GoDoc](https://godoc.org/github.com/bjlhlin/aliyungo/ram?status.svg)](https://godoc.org/github.com/bjlhlin/aliyungo/ram)
  * RDS: [https://godoc.org/github.com/bjlhlin/aliyungo/rds](https://godoc.org/github.com/bjlhlin/aliyungo/rds) [![GoDoc](https://godoc.org/github.com/bjlhlin/aliyungo/rds?status.svg)](https://godoc.org/github.com/bjlhlin/aliyungo/rds)
  * SLB: [https://godoc.org/github.com/bjlhlin/aliyungo/slb](https://godoc.org/github.com/bjlhlin/aliyungo/slb) [![GoDoc](https://godoc.org/github.com/bjlhlin/aliyungo/slb?status.svg)](https://godoc.org/github.com/bjlhlin/aliyungo/slb)
  * SLS: [https://godoc.org/github.com/bjlhlin/aliyungo/sls](https://godoc.org/github.com/bjlhlin/aliyungo/sls) [![GoDoc](https://godoc.org/github.com/bjlhlin/aliyungo/sls?status.svg)](https://godoc.org/github.com/bjlhlin/aliyungo/sls)
  * SMS: [https://godoc.org/github.com/bjlhlin/aliyungo/sms](https://godoc.org/github.com/bjlhlin/aliyungo/sms) [![GoDoc](https://godoc.org/github.com/bjlhlin/aliyungo/sms?status.svg)](https://godoc.org/github.com/bjlhlin/aliyungo/sms)
  * STS: [https://godoc.org/github.com/bjlhlin/aliyungo/sts](https://godoc.org/github.com/bjlhlin/aliyungo/sts) [![GoDoc](https://godoc.org/github.com/bjlhlin/aliyungo/sts?status.svg)](https://godoc.org/github.com/bjlhlin/aliyungo/sts)

## Build and Install

go get:

```sh
go get github.com/bjlhlin/aliyungo
```

## Test ECS

Modify "ecs/config_test.go"

```sh
	TestAccessKeyId     = "MY_ACCESS_KEY_ID"
	TestAccessKeySecret = "MY_ACCESS_KEY_ID"
	TestInstanceId      = "MY_INSTANCE_ID"
	TestIAmRich         = false
```

* TestAccessKeyId: the Access Key Id
* TestAccessKeySecret: the Access Key Secret.
* TestInstanceId: the existing instance id for testing. It will be stopped and restarted during testing.
* TestIAmRich(Optional): If it is set to true, it will perform tests to create virtual machines and disks under your account. And you will pay the bill. :-)

Under "ecs" and run

```sh
go test
```

## Test OSS

Modify "oss/config_test.go"

```sh
	TestAccessKeyId     = "MY_ACCESS_KEY_ID"
	TestAccessKeySecret = "MY_ACCESS_KEY_ID"
	TestRegion          = oss.Beijing
	TestBucket          = "bjlhlin"
```

* TestAccessKeyId: the Access Key Id
* TestAccessKeySecret: the Access Key Secret.
* TestRegion: the region of OSS for testing
* TestBucket: the bucket name for testing

Under "oss" and run

```sh
go test
```

## Contributors

  * Li Yi (bjlhlin@gmail.com)
  * Boshi Lian (farmer1992@gmail.com)
  * Yu Zhou (oscarrr110@gmail.com)
  * Yufei Zhang
  * linuxlikerqq
  * Changhai Yan
  * Jizhong Jiang (jiangjizhong@gmail.com)
  * Kent Wang (pragkent@gmail.com)
  * ringtail
  * aiden0z (aiden0xz@gmail.com)
  * jimmycmh
  * menglingwei
  * mingang.he (dustgle@gmail.com)
  * Young Chen (chainone@gmail.com)
  * johnzeng
  * spacexnice (445436286@qq.com)
  * xiaoheihero
  * hmgle (dustgle@gmail.com)
  * jzwlqx (jiangjizhong@gmail.com)
  * Linhua Tan (toolchainX@gmail.com)
  * Plutonist (p@vecsight.com)
  * Bin Liu
  * wangyue
  * demonwy
  * yarous224
  * yufeizyf (xazyf9111@sina.cn)
  * keontang (ikeontang@gmail.com)
  * Cholerae Hu (me@cholerae.com)
  * Zach Bergh (berghzach@gmail.com)
  * Bingshen Wang
  * xiaozhu36
  * Russell (yufeiwu@gmail.com)
  * zhuzhih2017
  * cheyang
  * Hobo Chen
  * Shuwei Yin
  * Xujin Zheng (xujinzheng@gmail.com)
  * Dino Lai (dinos80152@gmail.com)

## License

This project is licensed under the Apache License, Version 2.0. See [LICENSE](https://github.com/bjlhlin/aliyungo/blob/master/LICENSE.txt) for the full license text.

## Related projects

  * Aliyun ECS driver for Docker Machine: [Pull request](https://github.com/docker/machine/pull/1182)

  * Aliyun OSS driver for Docker Registry V2: [Pull request](https://github.com/docker/distribution/pull/514)

## References

The GO API design of OSS refer the implementation from [https://github.com/AdRoll/goamz](https://github.com/AdRoll)

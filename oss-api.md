# OSS 临时凭证获取 API 文档

## 📋 API 概述

**接口名称**: 获取阿里云 OSS 临时访问凭证  
**接口路径**: `GET /api/oss/token`  
**功能描述**: 通过阿里云 STS (Security Token Service) 服务获取临时访问凭证，用于客户端直接访问 OSS 存储桶

---

## 📤 请求信息

### 请求方式

### 请求参数
无需传入参数，所有配置通过服务端配置文件管理。

### 请求头

## 响应信息

### 成功响应 (200)

**响应格式**: JSON

```json
{
  "statusCode": "200",
  "accessKeyId": "STS.NUCxxxxxxxxxxxxxxx",
  "accessKeySecret": "xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
  "securityToken": "CAISxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
  "expiration": "2024-01-01T12:00:00Z",
  "endpoint": "oss-cn-shanghai.aliyuncs.com",
  "bucket": "your-bucket-name",
  "requestId": "61234567-89AB-CDEF-0123-456789ABCDEF"
}

```


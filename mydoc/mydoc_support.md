---
title: web
tags: [getting_started, troubleshooting]
keywords: questions, spark-java, contact, support
last_updated: March 20, 2016
summary: "Contact me for any support issues."
sidebar: mydoc_sidebar
permalink: /mydoc_support/
---

loginAction

[lavarel jwt ](https://github.com/jnuc093/study_quickstart-intermediate.git)

## spark-java

[spark-and-sql2o](https://sparktutorials.github.io/2015/04/29/spark-and-sql2o.html)

  本地数据库启动不需要带参数

    mvn exec:java --Dexec.args="--debug true"

  字段不对

    org.sql2o.Sql2oException: Could not map context to any property.

## MyBatis-Spring-Boot
➜  MyBatis-Spring-Boot git:(master) ✗ java -jar target/mybatis-spring-boot-1.0.0-SNAPSHOT.jar    

## jwt nimbus

    JWSObject jwsObject =JWSObject.parse(token);
    PayLoad payLoad = jwsObject.getPayload();
    JWSVerifier verifier = new MACVerifier(SECRET);

    if(jwsObject.verifier(verifier)){
      JSONObject jsonObject = payLoad.toJSONObject();
      HashMap<String,Object> test = jsonObject；

      resultMap.put("isSuccess",true);
      resultMap.put("data",jsonObject);
    }

new HashMap如何理解

    Map<String, Object> resultMap = new HashMap<String, Object>();


http://www.swiftsoftwaregroup.com/provision-chef-vagrant-omnibus-plugin/

sudo gitlab-ctl start

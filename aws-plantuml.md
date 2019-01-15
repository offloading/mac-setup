```uml
@startuml
!define AWSPUML https://raw.githubusercontent.com/milo-minderbinder/AWS-PlantUML/release/17-10-18/dist
!includeurl AWSPUML/common.puml
!includeurl AWSPUML/Storage/AmazonS3/AmazonS3.puml
!includeurl AWSPUML/Storage/AmazonS3/bucket/bucket.puml
!includeurl AWSPUML/General/user/user.puml
!includeurl AWSPUML/General/AWScloud/AWScloud.puml
!includeurl AWSPUML/NetworkingContentDelivery/AmazonCloudFront/AmazonCloudFront.puml

[BitBucket] as bitbucket
[CircleCI] as circleci

AWSCLOUD(aws) {
AMAZONS3(s3) {
BUCKET(blog, "akimoto.jp")
}

AMAZONCLOUDFRONT(cloudfront,"CDN")
}

:ユーザー: -right-> bitbucket :**1**) push
bitbucket -right-> circleci :**2**) kick
circleci -right-> blog :**3**) upload
blog --> cloudfront :**4**) distribute
:訪問者: .> cloudfront:閲覧

note "ビルド&テスト" as note_build_and_test
circleci .u. note_build_and_test
@enduml
```

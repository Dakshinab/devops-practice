# Task 02: S3 from the CLI

- Created a private S3 bucket in ap-south-1 with `aws s3 mb`
- Blocked all public access (`put-public-access-block`)
- Turned on versioning and uploaded two versions of the same file
- Deleted a file, saw the delete marker, and restored the file by removing the marker
- Synced a folder with `aws s3 sync` and confirmed that only changed files are uploaded
- Permanently deleted all versions, then deleted the bucket (no leftover cost)

What I learned: with versioning on, a normal delete only adds a delete marker. Only deleting a specific version ID is permanent.

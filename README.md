# vpc-tagging-ct-lifecycle-events
AWS solution for automatically tagging VPC resources based on Control Tower lifecycle event trigger. Leverages EventBridge, Lambda


# Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR APARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

# NOTES
This function can be adapted to run any code inside a newly created Control Tower Account. In this ****example****,we automatically tag the VPC resources (VPC, Subnets, Route Table, NAT Gateways, Internet Gateways, NACLs, default SG) for any default VPC created by Control Tower so users understand their function. Note that this code leverages the default 'AWSControlTowerExecution' role which is created automatically as part of Control Tower account provisioning.

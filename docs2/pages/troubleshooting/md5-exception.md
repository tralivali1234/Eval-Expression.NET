# MD5 Exception

## Problem

You execute a method from the Eval Expression.NET library, and the following error is thrown:

> This implementation is not part of the Windows Platform FIPS validated cryptographic algorithms.

## Solution

### Cause

The default algorithm to validate the license key & name is not supported with FIPS enabled.

### Fix

#### Ask for a compatible key

Contact us and we will send you a new key supporting FIPS: info@zzzprojects.com

Why don't we generate a key compatible with FIPS by default? Because it will not be supported for a client machine with Windows XP or below.

#### Disable FIPS

Article: [Disable FIPS](http://docs.trendmicro.com/all/ent/sc/v3.0/en-US/cmcolh/t_fips.html){:target="_blank"}

# AWS Cloud9 Setup Instructions

## Prerequisites
- Cornell NetID and password
- Duo Authentication enabled

## Getting Started

### 1. Initial Access
1. Access the AWS Console (link provided by instructor)
2. Log in using:
   - Cornell NetID
   - Password
   - Duo Authentication

### 2. Finding Cloud9
1. Once logged in to the AWS Console
2. Look for the search bar at the top
3. Type "Cloud9" (note: it's Cloud9, not Cloud0)

### 3. Instance Setup
1. Select a T3.nano instance
   - Cost-effective option
   - Automatically throttled for cost control
   - Minimal cost per half hour
2. Set timeout settings
   - Default is 30 minutes
   - System automatically shuts down after inactivity

### 4. Environment Configuration
- Login options:
  - Built-in AWS Cloud9 tools
  - SSH connection (alternative option)

### 5. Development Environment Features
- Similar to JupyterHub interface
- Can be configured as JupyterHub
- Supports custom environments:
  - Upload YAML configuration files
  - Import existing environment setups
  - Supports tools like:
    - PyTorch
    - NetCDF tools
    - Other scientific computing packages

### 6. Storage Options
- Limited local storage in home directories
- S3 bucket connection available:
  - Flexible storage (starting at 2GB)
  - Can be expanded as needed
  - Temporary storage solution
  - Data should be downloaded before bucket expiration

### 7. Additional Features
- VS Code integration:
  - Direct Cloud9 integration
  - SSH connection possible
- Regional server options (default: US East/Ohio node)

## Important Notes
- Users have administrator privileges
- Responsible for system security
- Environment is temporary and will shut down after inactivity
- Data should be backed up regularly
- Keep track of storage needs and communicate them to instructors

## Best Practices
1. Monitor usage time
2. Download important data regularly
3. Keep environment configurations backed up
4. Use cost-effective instance types
5. Shut down instances when not in use

## Support
Contact course instructor for:
- S3 bucket setup
- Storage expansion needs
- Access issues
- Configuration assistance

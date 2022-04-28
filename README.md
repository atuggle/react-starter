# React Starter

A Docker-based bootstrapper for a new React project.

This image uses the `create-react-app` command to create a new React app using the project name passed in as a command line parameter. Mapping a local volume to /project in the container causes the newly-created files to exist in that volume.

Helpful Docker Commands:

1. Build: 
    - `docker build -t atuggle/react-starter .`
2. Create local tag: 
    - `docker tag atuggle/react-starter react-starter:latest`
3. Push to docker hub: 
    - `docker push atuggle/react-starter:latest`
4. Run docker 
    = `docker run --rm -v $PWD:/project atuggle/react-starter react-demo`
5. Docker Compose build
    - `docker-compose build --no-cache`

## Quick Commands
- `docker build -t test-name .`
- `docker run test-name`
- `docker-compose logs -f web`
- `docker-compose exec web \bin\sh`
- `dc exec web sh`
# Storj DCS Public Network Statistics

This repository is designated to manage the work around providing official public statistics from Storj DCS satellites.

## Where is the service hosted?

You can access the service here: https://stats.storjshare.io/

The service is hosted as a [static website](https://docs.storj.io/dcs/how-tos/host-a-static-website) from a Storj DCS bucket.

## How to report a problem or an improvement request?

Open a [new issue](https://github.com/storj/stats/issues/new) to this repository.

## How to modify the website's homepage?

Edit the [homepage.md](homepage.md) file and open a pull request for review.

Once the pull request is merged, a [GitHub workflow](.github/workflows/upload-homepage.yml) that will automatically convert the Markdown file to an HTML file and will upload it to the bucket of the static website.

## Is there a better visualization of the data?

Yes, the Storj forum member [Arkina](https://forum.storj.io/u/Arkina) created a [Grafana dashboard](https://storjstats.info/) with better visualization of the data.

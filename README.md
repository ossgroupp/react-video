![alt text](https://raw.githubusercontent.com/ossgroupp/react-image/HEAD/media/logo.png 'An illustration of an atom')

# React Video for OSSPIM

A React package to output videos from OSSPIM using the native video element. Use this to easily embed videos powered by the [OSSPIM headless commerce service](https://ossgroup.com/).

## Demo

[Demo](https://react-video.milliseconds.io/)

## Install

```
yarn add @osspim/react-video
```

## Use

```
import { Video } from '@osspim/react-video';
import '@osspim/react-video/dist/styles.css';

const videoFromOSSPIM = {
    playlists: [...],
    thumbnails: [...]
}

<Video
    {...videoFromOSSPIM}
    thumbnmailProps={{sizes: "(max-width: 700px) 90vw, 700px" }}
/>
```

## Supported props

```
export interface Props extends HTMLAttributes<HTMLDivElement> {
  playlists: string[];
  thumbnails?: OSSPIMImageVariant[];
  thumbnailProps?: object;
  videoProps?: HTMLAttributes<HTMLVideoElement>;
  autoPlay?: boolean;
  loop?: boolean;
  muted?: boolean;
  controls?: boolean;
  poster?: string;
  playButtonText?: string;
}
```
# react-video

bakalım ne olacak



      run: docker build . --file golang/minideb/Dockerfile --tag ghcr.io/narslan/containers/golang:minideb-1.19.2
      with:
          repo-token: ${{ secrets.GITHUB_TOKEN }}
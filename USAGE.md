<!-- Start SDK Example Usage [usage] -->
```go
package main

import (
	"context"
	terraformprovideracmecheck "github.com/speakeasy-sdks/terraform-provider-acmecheck"
	"log"
	"net/http"
)

func main() {
	s := terraformprovideracmecheck.New()

	ctx := context.Background()
	res, err := s.Pets.CreatePets(ctx)
	if err != nil {
		log.Fatal(err)
	}

	if res.StatusCode == http.StatusOK {
		// handle response
	}
}

```
<!-- End SDK Example Usage [usage] -->
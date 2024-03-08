<!-- Start SDK Example Usage [usage] -->
```go
package main

import (
	"context"
	terraformprovideracmecheck "github.com/speakeasy-sdks/terraform-provider-acmecheck"
	"github.com/speakeasy-sdks/terraform-provider-acmecheck/pkg/models/shared"
	"log"
)

func main() {
	s := terraformprovideracmecheck.New()

	ctx := context.Background()
	res, err := s.Pets.CreatePets(ctx, shared.Pet{
		ID:   596804,
		Name: "<value>",
	})
	if err != nil {
		log.Fatal(err)
	}
	if res != nil {
		// handle response
	}
}

```
<!-- End SDK Example Usage [usage] -->
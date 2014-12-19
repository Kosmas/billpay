# Billpay

Supports payment capture and invoice creation:

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'billpay'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install billpay

## Usage

Capture payment:

    bill_pay = BillPay.new( order )
    bill_pay.capture

Invoice creation:

    bill_pay = BillPay.new( order )
    bill_pay.invoice_create

Require that order has specific structure, including associations with address, buyer, cart_entities.

ToDo:

  * Support DSL, which will allow to specify address buyer, cart_entities in dynamic way.
  * Logging responses
  * Refund functionality

## Contributing

1. Fork it ( https://github.com/[my-github-username]/billpay/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request
